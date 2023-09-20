# npm-package

## code blocks
    <html>
        <head></head>
    </html>

    function test() {
        console.log('test')
    }

this is so funny!  :joy:

## Specifying dependencies and devDependencies in a package.json file

- "dependencies": Packages required by your application in production.
- "devDependencies": Packages that are only needed for local development and testing.


 package file (package file)[https://juejin.cn/post/7240805459288522808]


认识 npm & yarn （二）安装依赖行为(认识 npm & yarn)[https://zhuanlan.zhihu.com/p/112237308]
>  npm install 一个包时： 
-  会同时引入这个包 dependencies 中的全部依赖
- 不会引入这个包 devDependencies 中的全部依赖
- 如果这个包包含了 peerDependencies，则会检查当前是否已引入相关依赖，如果没有则提示 warning

> 这里我们注意到 yarn 和 npm 安装的一个区别：
- yarn 引用一个包时，会将这个包的 dependencies 依赖放置和 包同级
- npm 引用一个包时，会将这个包的 dependencies 依赖放置在包的node_modules下