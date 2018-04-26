<template>
    <div class="check-list">
		<span v-for="(item,index) in list" :class="{checkedColor:item.status}" @click="changeStatus(item,index)" v-text="item.name">
		</span>
    </div>
</template>
<script>
    export default {
        data() {
            return {}
        },
        props: {
            list: {
                type: Array,
                default: []
            },
            checkedList: {
                type: Array,
                default: []
            },
            types: {
                type: String,
                default: 'radio'
            }
        },
        created: function () {
            this.list.map((item, index) => {
                if (this.checkedList.indexOf(Number(item.id)) > -1) {
                    this.$set(this.list[index], 'status', true)
                } else {
                    this.$set(this.list[index], 'status', false)
                }
                return item
            })
        },
        methods: {
            changeStatus(item, index) {
                if (this.types === 'radio') {
                    this.list.map((item) => {
                        item.status = false;
                    });
                    this.list[index].status = true;
                }
                else if (this.types === 'checkbox') {
                    if (item.status) {
                        item.status = false;
                        return
                    } else {
                        item.status = true;
                    }
                }else {

                }
                let newArr = [];
                this.list.map((item) => {
                    if (item.status) {
                        newArr.push(item.id);
                    }
                });
                this.$emit('sendCheckedList', newArr)
            }
        }
    }
</script>
<style>
    .checkedColor {
        background: #fcc;
        color: #fff;
    }

    span {
        float: left;
        margin-left: 10px;
        cursor: pointer;
    }
</style>
