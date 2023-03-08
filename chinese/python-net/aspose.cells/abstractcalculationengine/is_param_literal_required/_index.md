---
title: is_param_literal_required 属性
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 40
url: /zh/python-net/aspose.cells/abstractcalculationengine/is_param_literal_required/
is_root: false
---
## is_param_literal_required 属性

指示该引擎在计算时是否需要参数的文字文本。默认值为假。

### 评论

如果此自定义计算引擎需要参数的文字文本，则需要更多的堆栈来缓存参数的文字文本，并且可以递归调用 Calculate() 方法来计算参数的值。
通常计算公式不需要文字文本，对于大多数实现而言，此方法应返回 false 以获得更好的性能。
### 定义：
```python
@property
def is_param_literal_required(self):
    ...
```

### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [AbstractCalculationEngine](/cells/zh/python-net/aspose.cells/abstractcalculationengine)
