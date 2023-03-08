---
title: WorkbookDesigner类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 1600
url: /zh/python-net/aspose.cells/workbookdesigner/
is_root: false
---
##  WorkbookDesigner类
封装表示设计器电子表格的对象。



WorkbookDesigner 类型公开了以下成员：

### 构造器
|构造器|描述|
| :- | :- |
| [WorkbookDesigner()](/cells/zh/python-net/aspose.cells/workbookdesigner/__init__/#) |初始化 [WorkbookDesigner](/cells/zh/python-net/aspose.cells/workbookdesigner) 类的新实例。|
| [WorkbookDesigner(workbook)](/cells/zh/python-net/aspose.cells/workbookdesigner/__init__/#Workbook) |初始化 [WorkbookDesigner](/cells/zh/python-net/aspose.cells/workbookdesigner) 类的新实例。|


### 特性
|属性|描述|
| :- | :- |
| [workbook](/cells/zh/python-net/aspose.cells/workbookdesigner/workbook) |获取和设置 [WorkbookDesigner.workbook](/cells/zh/python-net/aspose.cells/workbookdesigner#workbook) 对象。|
| [repeat_formulas_with_subtotal](/cells/zh/python-net/aspose.cells/workbookdesigner/repeat_formulas_with_subtotal) |指示是否重复带有小计行的公式。|
| [update_empty_string_as_null](/cells/zh/python-net/aspose.cells/workbookdesigner/update_empty_string_as_null) |如果为 TRUE，如果值为 ""，将插入 Null；|
| [update_reference](/cells/zh/python-net/aspose.cells/workbookdesigner/update_reference) |指示是否更新其他工作表中的引用。|
| [calculate_formula](/cells/zh/python-net/aspose.cells/workbookdesigner/calculate_formula) |指示是否应计算公式。|
| [call_back](/cells/zh/python-net/aspose.cells/workbookdesigner/call_back) |获取和设置处理smartmarker的回调接口。|
| [line_by_line](/cells/zh/python-net/aspose.cells/workbookdesigner/line_by_line) |指示是否逐行处理智能标记。|


### 方法
|方法|描述|
| :- | :- |
| [set_data_source(data_source, cells_data_table)](/cells/zh/python-net/aspose.cells/workbookdesigner/set_data_source/#str-ICellsDataTable) |设置 [ICellsDataTable](/cells/zh/python-net/aspose.cells/icellsdatatable) 对象的数据源。|
| [set_data_source(variable, data)](/cells/zh/python-net/aspose.cells/workbookdesigner/set_data_source/#str-any) |将数据绑定设置为变量。|
| [process()](/cells/zh/python-net/aspose.cells/workbookdesigner/process/#) |处理智能标记并填充数据源值。|
| [process(is_preserved)](/cells/zh/python-net/aspose.cells/workbookdesigner/process/#bool) |处理智能标记并填充数据源值。|
| [process(sheet_index, is_preserved)](/cells/zh/python-net/aspose.cells/workbookdesigner/process/#int-bool) |处理智能标记并填充数据源值。|
| [clear_data_source()](/cells/zh/python-net/aspose.cells/workbookdesigner/clear_data_source/#) |清除所有数据源。|
| [get_smart_markers()](/cells/zh/python-net/aspose.cells/workbookdesigner/get_smart_markers/#) |返回电子表格中智能标记的集合。|



### 例子

```python
from aspose.cells import Workbook, WorkbookDesigner

# Create WorkbookDesigner object.
wd = WorkbookDesigner()
# Open the template file (which contains smart markers).
wd.workbook = Workbook("SmartMarker_Designer.xls")
# Initialize your data from data source
# DataSet ds = new DataSet();
# ...
# Set the datatable as the data source.
# wd.SetDataSource(dt);
# Process the smart markers to fill the data into the worksheets.
wd.process(True)
# Save the excel file.
wd.workbook.save("outSmartMarker_Designer.xls")

```

### 也可以看看
* 模块 [aspose.cells](..)
* 类 [ICellsDataTable](/cells/zh/python-net/aspose.cells/icellsdatatable)
* 类 [WorkbookDesigner](/cells/zh/python-net/aspose.cells/workbookdesigner)
