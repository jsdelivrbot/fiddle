```js
( {

    // modules 用于（在「项目构建模式」下）描述多个「入口文件」
    modules : [

        {

            // 待编译模块的模块标识；相对于 baseUrl 解析
            // 在描述「入口文件」时，name 为唯一的必须选项
            name : 'main' ,

            // 当待编译模块不存在时，是否创建一个空模块
            create : true ,

            // 引入指定模块及其依赖项
            include : [ 'foo' ] ,

            // 移除指定模块及其依赖项
            exclude : [ 'bar' ] ,
            // 移除指定模块，但不移除其依赖项
            excludeShallow : [ 'baz' ]

        }

    ] ,

    // 或（在「单文件构建模式」及「项目构建模式」下）描述单一「入口文件」
    name : 'main' ,
    create : true ,
    include : [ 'foo' ] ,
    exclude : [ 'bar' ] ,
    excludeShallow : [ 'baz' ]

} )
```

---

- [appDir](./appDir.md)
- [baseUrl](./baseUrl.md)
- [dir](./dir.md)
- [out](./out.md)
- [optimize](./optimize.md)
- [skipDirOptimize](./skipDirOptimize.md)
