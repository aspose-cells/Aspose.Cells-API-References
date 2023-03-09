---
title: invariant_custom 属性
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 260
url: /zh/python-net/aspose.cells/style/invariant_custom/
is_root: false
---
## invariant_custom 属性

获取数字格式的独立于文化的模式字符串。
如果没有为该对象设置数字格式，则返回 null。
如果内置数字格式，则返回内置数字对应的模式字符串。

### 评论

对于内置数字格式，返回的模式内容仍然依赖于文化，
例如，对于某些语言环境，它返回“m/d/y”，而对于其他一些语言环境，它返回“d/m/y”。
与 [Style.culture_custom](/cells/zh/python-net/aspose.cells/style#culture_custom) 的区别是（这也是与文化无关的意思）：
格式说明符和分隔符保持为标准，例如“/”将始终用作日期时间分隔符
并且“y”将始终用作“年”部分，而不管特定区域设置使用什么其他特殊字符。
### 定义：
```python
@property
def invariant_custom(self):
    ...
```

### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Style](/cells/zh/python-net/aspose.cells/style)
