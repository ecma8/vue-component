# 基于vue的loading组件 
## 本组件功能 
* 灵活分页
### html相关
```html
<loading v-if="isLoading"></loading>
```
### 结合vuex使用
## 优点如下
* 可一次引入 全局调用
* 结合vuex 只需要两个方法 一个变量就可以实现全局调用loading
* 相关配置稍微有些复杂 后续会补全