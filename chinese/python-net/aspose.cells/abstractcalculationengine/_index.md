---
title: AbstractCalculationEngine类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 20
url: /zh/python-net/aspose.cells/abstractcalculationengine/
is_root: false
---
## AbstractCalculationEngine类
代表用户自定义计算引擎，扩展Aspose.Cells默认计算引擎。



AbstractCalculationEngine 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [is_param_literal_required](/cells/zh/python-net/aspose.cells/abstractcalculationengine/is_param_literal_required) |指示该引擎在计算时是否需要参数的文字文本。默认值为假。|
| [process_built_in_functions](/cells/zh/python-net/aspose.cells/abstractcalculationengine/process_built_in_functions) |内置引擎已经支持的内置函数是否应该被这个实现检查和处理。<br/>默认为假。<br/>如果用户需要更改某些内置函数的计算逻辑，则应将此属性设置为 true。|


### 方法
|方法|描述|
| :- | :- |
| [calculate(data)](/cells/zh/python-net/aspose.cells/abstractcalculationengine/calculate/#CalculationData) |使用给定数据计算一个函数。|



### 评论

用户不应在此实现中直接修改工作簿的任何部分（自定义函数的计算结果除外，可通过 CalculationData.CalculatedValue 属性设置）。
否则可能导致意想不到的结果或异常。
如果用户在某些自定义函数的实现中需要更改计算结果以外的其他数据，
例如，更改单元格的公式、样式等，用户应在此实现中收集这些数据，并在公式计算范围之外进行更改。

### 也可以看看
* 模块 [aspose.cells](..)
