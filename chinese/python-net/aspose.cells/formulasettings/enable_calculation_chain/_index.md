---
title: enable_calculation_chain 属性
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 70
url: /zh/python-net/aspose.cells/formulasettings/enable_calculation_chain/
is_root: false
---
## enable_calculation_chain 属性

是否为公式启用计算链。默认为假。

### 评论

当工作簿中的公式较多，需要反复计算时
只修改其中的一小部分，启用计算链可能对性能有帮助。
另一方面，如果启用链，维护链的模型需要额外的内存，
并且它还需要更多的 CPU 时间来执行其他一些操作，例如更改单元格的值或公式。
将这个属性从false改为true后，会分析构建计算链
在第一次计算工作簿时，所以第一次计算所需的时间
可能比正常计算更不用链。
### 定义：
```python
@property
def enable_calculation_chain(self):
    ...
@enable_calculation_chain.setter
def enable_calculation_chain(self, value):
    ...
```

### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [FormulaSettings](/cells/zh/python-net/aspose.cells/formulasettings)
