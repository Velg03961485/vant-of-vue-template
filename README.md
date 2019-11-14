# vant-of-vue-template
use vant of vue cretaed  ios/android application



### 安装


需要在vue cli3 以上才能安装


npm install -g @vue/cli


vue create template


npm i vant -S


 cd template
 
 
 npm run serve
 
 
 
 ###开发历程
 
 
 .按需引入css
 
 
 npm i babel-plugin-import -D
 
 然后找到 babel.config.js 文件，添加
 
 
 ```
    module.exports = {
        plugins: [
            ['import',{
                libraryName: 'vant',
                libraryDirectory: 'es',
                style: true
            },'vant']
        ],
    };


```


在需要的文件中，挨个引入需要的组件

```javascript
import {button} from 'vant'
```



.安装router

由于失误操作，安装vue-router的时候一直报错

This is related to npm not being able to find a file

删除 node_modules 文件

npm install

npm install vue-router


 
 
