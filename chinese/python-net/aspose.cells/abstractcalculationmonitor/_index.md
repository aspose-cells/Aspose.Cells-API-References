---
title: AbstractCalculationMonitor类
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 30
url: /zh/python-net/aspose.cells/abstractcalculationmonitor/
is_root: false
---
## AbstractCalculationMonitor类
监视用户以跟踪公式计算的进度。



AbstractCalculationMonitor 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [original_value](/cells/zh/python-net/aspose.cells/abstractcalculationmonitor/original_value) |获取计算单元格的旧值。<br/>应仅在 [AbstractCalculationMonitor.before_calculate(sheet_index, row_index, col_index)](/cells/zh/python-net/aspose.cells/abstractcalculationmonitor/before_calculate) 和 [AbstractCalculationMonitor.after_calculate(sheet_index, row_index, col_index)](/cells/zh/python-net/aspose.cells/abstractcalculationmonitor/after_calculate) 中使用。|
| [value_changed](/cells/zh/python-net/aspose.cells/abstractcalculationmonitor/value_changed) |计算后单元格的值是否已更改。<br/>应仅在 [AbstractCalculationMonitor.after_calculate(sheet_index, row_index, col_index)](/cells/zh/python-net/aspose.cells/abstractcalculationmonitor/after_calculate) 中使用。|
| [calculated_value](/cells/zh/python-net/aspose.cells/abstractcalculationmonitor/calculated_value) |获取单元格的新计算值。<br/>应仅在 [AbstractCalculationMonitor.after_calculate(sheet_index, row_index, col_index)](/cells/zh/python-net/aspose.cells/abstractcalculationmonitor/after_calculate) 中使用。|


### 方法
|方法|描述|
| :- | :- |
| [before_calculate(sheet_index, row_index, col_index)](/cells/zh/python-net/aspose.cells/abstractcalculationmonitor/before_calculate/#int-int-int) |在计算一个单元格之前执行此方法来处理业务。|
| [after_calculate(sheet_index, row_index, col_index)](/cells/zh/python-net/aspose.cells/abstractcalculationmonitor/after_calculate/#int-int-int) |计算完一个单元格后执行此方法进行业务。|
| [on_circular(circular_cells_data)](/cells/zh/python-net/aspose.cells/abstractcalculationmonitor/on_circular/#collections.abc.Iterator) |在计算循环引用的公式时实现这个方法来做业务。|



### 也可以看看
* 模块 [aspose.cells](..)
