# 基于vue的分页组件 
## 本组件功能 
### html相关
```html
	<page :pages=10 :curr=1 v-on:pageIndex="pageIndex"></page>
```
```javscript
methods:{
    pageIndex(data){
        
    }
}
```
## 插件配置 
* pages 为总页数  
* curr为当前页面 
* v-on:pageIndex接收子组件发来的页码
### javascript相关
