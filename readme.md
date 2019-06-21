## 项目说明

### 编译打包

npm install  <br/>
npm run build

### 目录结构
```
|-- common
|   `-- loader.js                       //公共部分
|-- lib                                 //导出目录
|   |-- Animate                         //动画库
|   |   `-- index.js
|   |-- Editor                          //编辑
|   |   |-- game                        //编辑游戏页
|   |   |   `-- index.js
|   |   |-- render                      //渲染
|   |   |   |-- DragElement.js
|   |   |   `-- index.js
|   |   |-- start                       //编辑开始页
|   |   |   `-- index.js    
|   |   `-- subtitle                    //编辑题干部分
|   |       `-- index.js
|   |-- Preview                         //预览
|   |   |-- game
|   |   |   `-- index.js                //预览游戏页
|   |   |-- start
|   |   |   `-- index.js                //预览开始页
|   |   `-- subtitle
|   |       `-- index.js                //预览题干部分
|   |-- index.js
|   `-- packages
|       |-- Editor
|       |   `-- index.js
|       `-- Preview
|           `-- index.js
|-- package-lock.json
|-- package.json
|-- README.md
|-- src                                  //原始目录
|   |-- Animate                          //动画库   
|   |   |-- index.js
|   |   `-- readme.md
|   |-- Editor                           //编辑
|   |   |-- game                         //编辑游戏页
|   |   |   `-- index.js
|   |   |-- render                       //渲染
|   |   |   |-- DragElement.js
|   |   |   `-- index.js
|   |   |-- start                        //编辑开始页
|   |   |   `-- index.js
|   |   `-- subtitle                     //编辑题干部分
|   |       `-- index.js
|   |-- Preview                          //预览
|   |   |-- game                         //预览游戏页
|   |   |   `-- index.js
|   |   |-- start                        //预览开始页
|   |   |   `-- index.js
|   |   `-- subtitle                     //预览题干部分
|   |       `-- index.js
|   |-- index.js
|   `-- packages                         //vue预览编辑页面
|       |-- Editor                       //编辑页面
|       |   |-- index.js
|       |   `-- src
|       |       |-- Edit.vue
|       |       |-- EditEnd.vue
|       |       |-- EditGame.vue
|       |       |-- EditGamePublic.vue
|       |       |-- EditPreview.vue
|       |       `-- EditStart.vue
|       `-- Preview                      //预览页面
|           |-- index.js
|           `-- src
|               `-- Preview.vue
```