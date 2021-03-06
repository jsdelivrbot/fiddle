[map](http://requirejs.org/docs/api.html#config-map) 用于设置指定模块（集）下的路径/模块别名

> - 结构化匹配
> - `paths` 用于设置通用路径/模块别名，而 `map` 则用于设置指定模块（集）下的路径/模块别名
> - 不支持 `path-fallback`

```js
require.config( {
    map : {

        // 通用路径/模块别名
        // 此时等同于 paths 配置项
        '*' : {
            foo : 'bar'
        } ,

        // 指定模块（集）下的路径/模块别名
        // 覆盖通用路径/模块别名
        prefix : {
            foo : 'bar'
        }

    }
} )
```

> 相关配置项：[paths](./paths.md)
