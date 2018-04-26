# 基于vue的分页组件 
## 本组件功能 
### html相关
```html
	<check-box :list="goodsType" :checkedList="goodsSelect" @sendCheckedList="getCheckedList" types='radio'></check-box>
```
```javscript
methods:{
    getCheckedList(data){
        //返回值是数组 如果要传后台 调用toString()方法就可以了
    }
}
```
## 插件配置 
* list 所有的按钮数据
* checkedList 选中的列表id 单选只能传一个值
* types 单选复选状态 单选为radio 复选为checkbox
* getCheckedList 获取选中的按钮列表
