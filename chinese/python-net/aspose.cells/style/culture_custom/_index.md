---
title: culture_custom 属性
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 170
url: /zh/python-net/aspose.cells/style/culture_custom/
is_root: false
---
## culture_custom 属性

获取和设置数字格式的区域性相关模式字符串。
如果没有为该对象设置数字格式，则返回 null。
如果内置数字格式，则返回内置数字对应的模式字符串。

### 评论

对于内置数字格式，模式内容（例如，对于某些语言环境，一种内置日期格式是“m/d/y”，
但对于其他一些语言环境，它变为“d/m/y”）和格式说明符（例如，
某些语言环境使用“y”以外的字符来表示日期格式的年份部分）
依赖于文化；
对于用户指定的自定义格式，只有格式说明符会根据文化发生变化，
格式化模式的其他部分不会被修改。
### 定义：
```python
@property
def culture_custom(self):
    ...
@culture_custom.setter
def culture_custom(self, value):
    ...
```

### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Style](/cells/zh/python-net/aspose.cells/style)
