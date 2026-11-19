---
title: "WorkbookDesigner"
second_title: "Aspose.Cells for Java API 参考"
description: "封装表示设计器电子表格的对象。"
type: docs
url: /zh/java/com.aspose.cells/workbookdesigner/
---

**Inheritance:**
java.lang.Object
```
public class WorkbookDesigner
```

封装表示设计器电子表格的对象。

**Example**

```
         //Create WorkbookDesigner object.
         WorkbookDesigner wd = new WorkbookDesigner();
         //Open the template file (which contains smart markers).
         wd.setWorkbook(new Workbook("SmartMarker_Designer.xls"));
 
         //Initialize your data from data source
         //DataSet ds = new DataSet();
 
 
         //Set the datatable as the data source.
         //wd.SetDataSource(dt);
         //Process the smart markers to fill the data into the worksheets.
         wd.process(true);
         //Save the excel file.
         wd.getWorkbook().save("outSmartMarker_Designer.xls");
```
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [WorkbookDesigner()](#WorkbookDesigner--) | 初始化 [WorkbookDesigner](../../com.aspose.cells/workbookdesigner) 类的新实例。 |
| [WorkbookDesigner(Workbook workbook)](#WorkbookDesigner-com.aspose.cells.Workbook-) | 初始化 [WorkbookDesigner](../../com.aspose.cells/workbookdesigner) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [clearDataSource()](#clearDataSource--) | 清除所有数据源。 |
| [containsVariables()](#containsVariables--) | 指示第一个工作表是否包含自定义变量。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculateFormula()](#getCalculateFormula--) | 指示是否应计算公式。 |
| [getCallBack()](#getCallBack--) | 获取处理 smartmarker 的回调接口。 |
| [getClass()](#getClass--) |  |
| [getEnableHeaderFooterMarkers()](#getEnableHeaderFooterMarkers--) | 指示页眉/页脚是否包含智能标记以及是否应一起处理。 |
| [getLineByLine()](#getLineByLine--) | 指示是否逐行处理智能标记。 |
| [getRepeatFormulasWithSubtotal()](#getRepeatFormulasWithSubtotal--) | 指示是否在小计行中重复公式。 |
| [getSmartMarkers()](#getSmartMarkers--) | 返回电子表格中智能标记的集合。 |
| [getSortDataSource()](#getSortDataSource--) | 指示是否对数据源进行排序。 |
| [getUpdateEmptyStringAsNull()](#getUpdateEmptyStringAsNull--) | 如果为 TRUE，则在值为 "" 时插入 Null； |
| [getUpdateReference()](#getUpdateReference--) | 指示是否会更新其他工作表中的引用。 |
| [getVariablesWorksheetName()](#getVariablesWorksheetName--) | 获取包含变量智能标记的工作表名称。 |
| [getWorkbook()](#getWorkbook--) | 获取 [getWorkbook()](../../com.aspose.cells/workbookdesigner\#getWorkbook--) 对象。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [process()](#process--) | 处理智能标记并填充数据源值。 |
| [process(boolean isPreserved)](#process-boolean-) | 处理智能标记并填充数据源值。 |
| [process(Range range, boolean isPreserved)](#process-com.aspose.cells.Range-boolean-) | 处理智能标记并填充数据源值。 |
| [process(int sheetIndex, boolean isPreserved)](#process-int-boolean-) | 处理智能标记并填充数据源值。 |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | 指示是否应计算公式。 |
| [setCallBack(ISmartMarkerCallBack value)](#setCallBack-com.aspose.cells.ISmartMarkerCallBack-) | 设置处理智能标记的回调接口。 |
| [setContainsVariables(boolean value)](#setContainsVariables-boolean-) | 指示第一个工作表是否包含自定义变量。 |
| [setDataSource(String dataSource, ICellsDataTable cellsDataTable)](#setDataSource-java.lang.String-com.aspose.cells.ICellsDataTable-) | 设置 [ICellsDataTable](../../com.aspose.cells/icellsdatatable) 对象的数据源。 |
| [setDataSource(String variable, Object data)](#setDataSource-java.lang.String-java.lang.Object-) | 设置对变量的数据绑定。 |
| [setDataSource(String dataSource, ResultSet rs)](#setDataSource-java.lang.String-java.sql.ResultSet-) | 设置数据源。 |
| [setDataSource(String dataSource, ResultSet rs, int rowCount)](#setDataSource-java.lang.String-java.sql.ResultSet-int-) | 设置数据源。 |
| [setDataSource(ResultSet rs)](#setDataSource-java.sql.ResultSet-) | 设置数据源。 |
| [setEnableHeaderFooterMarkers(boolean value)](#setEnableHeaderFooterMarkers-boolean-) | 指示页眉/页脚是否包含智能标记以及是否应一起处理。 |
| [setJsonDataSource(String name, String json)](#setJsonDataSource-java.lang.String-java.lang.String-) | 将 JSON 字符串值设为智能标记的数据源。 |
| [setLineByLine(boolean value)](#setLineByLine-boolean-) | 指示是否逐行处理智能标记。 |
| [setRepeatFormulasWithSubtotal(boolean value)](#setRepeatFormulasWithSubtotal-boolean-) | 指示是否在小计行中重复公式。 |
| [setSortDataSource(boolean value)](#setSortDataSource-boolean-) | 指示是否对数据源进行排序。 |
| [setUpdateEmptyStringAsNull(boolean value)](#setUpdateEmptyStringAsNull-boolean-) | 如果为 TRUE，则在值为 "" 时插入 Null； |
| [setUpdateReference(boolean value)](#setUpdateReference-boolean-) | 指示是否会更新其他工作表中的引用。 |
| [setVariablesWorksheetName(String value)](#setVariablesWorksheetName-java.lang.String-) | 设置包含变量智能标记的工作表名称。 |
| [setWorkbook(Workbook value)](#setWorkbook-com.aspose.cells.Workbook-) | 设置 [getWorkbook()](../../com.aspose.cells/workbookdesigner\#getWorkbook--) 对象。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### WorkbookDesigner() {#WorkbookDesigner--}
```
public WorkbookDesigner()
```


初始化 [WorkbookDesigner](../../com.aspose.cells/workbookdesigner) 类的新实例。

### WorkbookDesigner(Workbook workbook) {#WorkbookDesigner-com.aspose.cells.Workbook-}
```
public WorkbookDesigner(Workbook workbook)
```


初始化 [WorkbookDesigner](../../com.aspose.cells/workbookdesigner) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| workbook | [Workbook](../../com.aspose.cells/workbook) | 模板工作簿文件。 |

### clearDataSource() {#clearDataSource--}
```
public void clearDataSource()
```


清除所有数据源。

### containsVariables() {#containsVariables--}
```
public boolean containsVariables()
```


指示第一个工作表是否包含自定义变量。

**Remarks**

NOTE: 此成员现已过时。请改用 WorkbookDesigner.VariablesWorksheetName 属性。该属性将在自 2025 年 9 月起的 3 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
boolean
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getCalculateFormula() {#getCalculateFormula--}
```
public boolean getCalculateFormula()
```


指示是否应计算公式。

**Returns:**
boolean
### getCallBack() {#getCallBack--}
```
public ISmartMarkerCallBack getCallBack()
```


获取处理 smartmarker 的回调接口。

**Returns:**
[ISmartMarkerCallBack](../../com.aspose.cells/ismartmarkercallback)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEnableHeaderFooterMarkers() {#getEnableHeaderFooterMarkers--}
```
public boolean getEnableHeaderFooterMarkers()
```


指示页眉/页脚是否包含智能标记以及是否应一起处理。

**Returns:**
boolean
### getLineByLine() {#getLineByLine--}
```
public boolean getLineByLine()
```


指示是否逐行处理智能标记。

**Remarks**

NOTE: 此类现已过时。请改用范围智能标记。该属性将在自 2025 年 7 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
boolean
### getRepeatFormulasWithSubtotal() {#getRepeatFormulasWithSubtotal--}
```
public boolean getRepeatFormulasWithSubtotal()
```


指示是否在小计行中重复公式。

**Returns:**
boolean
### getSmartMarkers() {#getSmartMarkers--}
```
public String[] getSmartMarkers()
```


返回电子表格中智能标记的集合。

**Remarks**

每次调用时都会创建字符串数组。该数组已排序并删除重复值。

**Returns:**
java.lang.String[] - 智能标记的集合
### getSortDataSource() {#getSortDataSource--}
```
public boolean getSortDataSource()
```


指示是否对数据源进行排序。

**Remarks**

NOTE: 此属性现已过时。该属性将在自 2026 年 10 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。如果智能标记包含升序和降序参数，JSON 数据源将被排序。

**Returns:**
boolean
### getUpdateEmptyStringAsNull() {#getUpdateEmptyStringAsNull--}
```
public boolean getUpdateEmptyStringAsNull()
```


如果为 TRUE，则在值为 "" 时插入 Null；

**Returns:**
boolean
### getUpdateReference() {#getUpdateReference--}
```
public boolean getUpdateReference()
```


指示是否会更新其他工作表中的引用。

**Returns:**
boolean
### getVariablesWorksheetName() {#getVariablesWorksheetName--}
```
public String getVariablesWorksheetName()
```


获取包含变量智能标记的工作表名称。

**Returns:**
java.lang.String
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


获取 [getWorkbook()](../../com.aspose.cells/workbookdesigner\#getWorkbook--) 对象。

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### process() {#process--}
```
public void process()
```


处理智能标记并填充数据源值。

### process(boolean isPreserved) {#process-boolean-}
```
public void process(boolean isPreserved)
```


处理智能标记并填充数据源值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| isPreserved | boolean | 如果未识别的智能标记被保留，则为 True。 |

### process(Range range, boolean isPreserved) {#process-com.aspose.cells.Range-boolean-}
```
public void process(Range range, boolean isPreserved)
```


处理智能标记并填充数据源值。

**Remarks**

NOTE: 此类现已过时。请改用 Range 智能标记。该属性将在自 2025 年 7 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | 要处理的范围 |
| isPreserved | boolean | 如果未识别的智能标记被保留，则为 True。 |

### process(int sheetIndex, boolean isPreserved) {#process-int-boolean-}
```
public void process(int sheetIndex, boolean isPreserved)
```


处理智能标记并填充数据源值。

**Remarks**

此方法在工作表级别上工作。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sheetIndex | int | 工作表索引。 |
| isPreserved | boolean | 如果未识别的智能标记被保留，则为 True。 |

### setCalculateFormula(boolean value) {#setCalculateFormula-boolean-}
```
public void setCalculateFormula(boolean value)
```


指示是否应计算公式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setCallBack(ISmartMarkerCallBack value) {#setCallBack-com.aspose.cells.ISmartMarkerCallBack-}
```
public void setCallBack(ISmartMarkerCallBack value)
```


设置处理智能标记的回调接口。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [ISmartMarkerCallBack](../../com.aspose.cells/ismartmarkercallback) |  |

### setContainsVariables(boolean value) {#setContainsVariables-boolean-}
```
public void setContainsVariables(boolean value)
```


指示第一个工作表是否包含自定义变量。

**Remarks**

NOTE: 此成员现已过时。请改用 WorkbookDesigner.VariablesWorksheetName 属性。该属性将在自 2025 年 9 月起的 3 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setDataSource(String dataSource, ICellsDataTable cellsDataTable) {#setDataSource-java.lang.String-com.aspose.cells.ICellsDataTable-}
```
public void setDataSource(String dataSource, ICellsDataTable cellsDataTable)
```


设置 [ICellsDataTable](../../com.aspose.cells/icellsdatatable) 对象的数据源。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| dataSource | java.lang.String | 数据源的名称。 |
| cellsDataTable | [ICellsDataTable](../../com.aspose.cells/icellsdatatable) | 数据表。 |

### setDataSource(String variable, Object data) {#setDataSource-java.lang.String-java.lang.Object-}
```
public void setDataSource(String variable, Object data)
```


设置对变量的数据绑定。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 变量 | java.lang.String | 使用智能标记创建的变量名。 |
| 数据 | java.lang.Object | 源数据。 |

### setDataSource(String dataSource, ResultSet rs) {#setDataSource-java.lang.String-java.sql.ResultSet-}
```
public void setDataSource(String dataSource, ResultSet rs)
```


设置数据源。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| dataSource | java.lang.String | 数据源的名称。 |
| rs | java.sql.ResultSet | 结果集。 |

### setDataSource(String dataSource, ResultSet rs, int rowCount) {#setDataSource-java.lang.String-java.sql.ResultSet-int-}
```
public void setDataSource(String dataSource, ResultSet rs, int rowCount)
```


设置数据源。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| dataSource | java.lang.String | 数据源的名称。 |
| rs | java.sql.ResultSet | 结果集。 |
| rowCount | int | 给定结果集的数据计数。它应为精确的行数或 -1；如果结果集是只向前的，用户应在此提供精确的行数，否则当智能标记的 "noadd" 未设置时，智能可能无法正确处理。 |

### setDataSource(ResultSet rs) {#setDataSource-java.sql.ResultSet-}
```
public void setDataSource(ResultSet rs)
```


设置数据源。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rs | java.sql.ResultSet | 结果集。 |

### setEnableHeaderFooterMarkers(boolean value) {#setEnableHeaderFooterMarkers-boolean-}
```
public void setEnableHeaderFooterMarkers(boolean value)
```


指示页眉/页脚是否包含智能标记以及是否应一起处理。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setJsonDataSource(String name, String json) {#setJsonDataSource-java.lang.String-java.lang.String-}
```
public void setJsonDataSource(String name, String json)
```


将 JSON 字符串值设为智能标记的数据源。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 表的名称。如果 JSON 的值表示一个对象，它可能为 null。 |
| json | java.lang.String | Json 字符串的值。 |

### setLineByLine(boolean value) {#setLineByLine-boolean-}
```
public void setLineByLine(boolean value)
```


指示是否逐行处理智能标记。

**Remarks**

NOTE: 此类现已过时。请改用范围智能标记。该属性将在自 2025 年 7 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setRepeatFormulasWithSubtotal(boolean value) {#setRepeatFormulasWithSubtotal-boolean-}
```
public void setRepeatFormulasWithSubtotal(boolean value)
```


指示是否在小计行中重复公式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSortDataSource(boolean value) {#setSortDataSource-boolean-}
```
public void setSortDataSource(boolean value)
```


指示是否对数据源进行排序。

**Remarks**

NOTE: 此属性现已过时。该属性将在自 2026 年 10 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。如果智能标记包含升序和降序参数，JSON 数据源将被排序。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setUpdateEmptyStringAsNull(boolean value) {#setUpdateEmptyStringAsNull-boolean-}
```
public void setUpdateEmptyStringAsNull(boolean value)
```


如果为 TRUE，则在值为 "" 时插入 Null；

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setUpdateReference(boolean value) {#setUpdateReference-boolean-}
```
public void setUpdateReference(boolean value)
```


指示是否会更新其他工作表中的引用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setVariablesWorksheetName(String value) {#setVariablesWorksheetName-java.lang.String-}
```
public void setVariablesWorksheetName(String value)
```


设置包含变量智能标记的工作表名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setWorkbook(Workbook value) {#setWorkbook-com.aspose.cells.Workbook-}
```
public void setWorkbook(Workbook value)
```


设置 [getWorkbook()](../../com.aspose.cells/workbookdesigner\#getWorkbook--) 对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Workbook](../../com.aspose.cells/workbook) |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

