antd 样式按需引入：
   yarn add antd
   import { Button } from 'antd'

   安装 yarn add react-app-rewired customize-cra

   新建并配置config-overrides.js文件 

   配置具体的修改规则
   const { override, fixBabelImports} = require('customize-cra')
   module.exports = override(
   fixBabelImports('import', {
    libraryName: 'antd',
    libraryDirectory: 'es',
    style: 'css',
	})
    );
     yarn add babel-plugin-import
     修改配置文件package.json中的start bulid test文件中的 react-app-rewired start/build/test
    

路由表

生成路由规则，只需要一个“element作为跳转的路由注册”

npm i react-router-dom

import { BrowserRouter } from 'react-router-dom'

index.ts里面BrowserRouter标签包裹App组件
