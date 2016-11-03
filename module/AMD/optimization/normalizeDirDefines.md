```js
( {

    // normalizeDirDefines 用于设置在「项目构建模式」下，是否将 modules 选项之外的脚本转换为标准 AMD 模块（分析局部 require 调用并将依赖显式放入 deps 实参中）
    normalizeDirDefines : 'skip'

} )
```

> - 当 `optimize == 'none'` 时，自动设为 `'skip'`
> - 当 `optimize != 'none' && skipDirOptimize == false` 时，自动设为 `'all'`

---

相关选项：

- [dir](./dir.md)
- [optimize](./optimize.md)
- [skipDirOptimize](./skipDirOptimize.md)