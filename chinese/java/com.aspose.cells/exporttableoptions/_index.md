---
title: "ExportTableOptions"
second_title: "Aspose.Cells for Java API 参考"
description: "表示所有导出表选项。"
type: docs
url: /zh/java/com.aspose.cells/exporttableoptions/
---

**Inheritance:**
java.lang.Object
```
public class ExportTableOptions
```

表示所有导出表选项。

**Remarks**

如果对导出有一些特殊要求，例如忽略错误值，用户可以扩展此类以覆盖相应的 API 来实现目标。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [ExportTableOptions()](#ExportTableOptions--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllowDBNull()](#getAllowDBNull--) | 此值指示是否允许在此表中使用 DBNull。 |
| [getCheckMixedValueType()](#getCheckMixedValueType--) | False，Aspose.Cells 将根据第一行的值类型设置 DataColumn 的类型以提升性能。 |
| [getClass()](#getClass--) |  |
| [getExportAsHtmlString()](#getExportAsHtmlString--) | 将单元格的 HTML 字符串值导出到 DataTable。 |
| [getExportAsString()](#getExportAsString--) | 将单元格的字符串值导出到 DataTable。 |
| [getExportColumnName()](#getExportColumnName--) | 指示是否将第一行的数据导出为 DataTable 的列名。 |
| [getFormatStrategy()](#getFormatStrategy--) | 获取将值导出为字符串时的格式策略。 |
| [getIndexes()](#getIndexes--) | 应导出的列/行的索引。 |
| [getPlotVisibleCells()](#getPlotVisibleCells--) | 仅导出可见单元格。 |
| [getPlotVisibleColumns()](#getPlotVisibleColumns--) | 仅导出可见列。 |
| [getPlotVisibleRows()](#getPlotVisibleRows--) | 仅导出可见行。 |
| [getRenameStrategy()](#getRenameStrategy--) | 列重复名称的策略。 |
| [getSkipErrorValue()](#getSkipErrorValue--) | 指示是否跳过列的无效值。 |
| [hashCode()](#hashCode--) |  |
| [isVertical()](#isVertical--) | True，如果工作簿文件中的一行对应 DataTable 中的一行。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [preprocessExportedValue(int cellRow, int cellColumn, CellValue value)](#preprocessExportedValue-int-int-com.aspose.cells.CellValue-) | 预处理当前单元格的待导出值。 |
| [setAllowDBNull(boolean value)](#setAllowDBNull-boolean-) | 此值指示是否允许在此表中使用 DBNull。 |
| [setCheckMixedValueType(boolean value)](#setCheckMixedValueType-boolean-) | False，Aspose.Cells 将根据第一行的值类型设置 DataColumn 的类型以提升性能。 |
| [setExportAsHtmlString(boolean value)](#setExportAsHtmlString-boolean-) | 将单元格的 HTML 字符串值导出到 DataTable。 |
| [setExportAsString(boolean value)](#setExportAsString-boolean-) | 将单元格的字符串值导出到 DataTable。 |
| [setExportColumnName(boolean value)](#setExportColumnName-boolean-) | 指示是否将第一行的数据导出为 DataTable 的列名。 |
| [setFormatStrategy(int value)](#setFormatStrategy-int-) | 设置将值导出为字符串时的格式策略。 |
| [setIndexes(int[] value)](#setIndexes-int---) | 应导出的列/行的索引。 |
| [setPlotVisibleCells(boolean value)](#setPlotVisibleCells-boolean-) | 仅导出可见单元格。 |
| [setPlotVisibleColumns(boolean value)](#setPlotVisibleColumns-boolean-) | 仅导出可见列。 |
| [setPlotVisibleRows(boolean value)](#setPlotVisibleRows-boolean-) | 仅导出可见行。 |
| [setRenameStrategy(int value)](#setRenameStrategy-int-) | 列重复名称的策略。 |
| [setSkipErrorValue(boolean value)](#setSkipErrorValue-boolean-) | 指示是否跳过列的无效值。 |
| [setVertical(boolean value)](#setVertical-boolean-) | True，如果工作簿文件中的一行对应 DataTable 中的一行。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ExportTableOptions() {#ExportTableOptions--}
```
public ExportTableOptions()
```


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
### getAllowDBNull() {#getAllowDBNull--}
```
public boolean getAllowDBNull()
```


此值指示是否允许在此表中使用 DBNull。

**Returns:**
boolean
### getCheckMixedValueType() {#getCheckMixedValueType--}
```
public boolean getCheckMixedValueType()
```


False，Aspose.Cells 将根据第一行的值类型设置 DataColumn 的类型以提升性能。True，Aspose.Cells 会在设置 DataColumn 的类型之前检查列中的值类型是否混合；如果值类型混合，DataColumn 的类型将为 string。

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getExportAsHtmlString() {#getExportAsHtmlString--}
```
public boolean getExportAsHtmlString()
```


将单元格的 HTML 字符串值导出到 DataTable。

**Returns:**
boolean
### getExportAsString() {#getExportAsString--}
```
public boolean getExportAsString()
```


将单元格的字符串值导出到 DataTable。

**Returns:**
boolean
### getExportColumnName() {#getExportColumnName--}
```
public boolean getExportColumnName()
```


指示是否将第一行的数据导出为 DataTable 的列名。默认值为 false。

**Returns:**
boolean
### getFormatStrategy() {#getFormatStrategy--}
```
public int getFormatStrategy()
```


获取将值导出为字符串时的格式策略。

参见 [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy)。

**Remarks**

默认值是 [CellValueFormatStrategy.CELL\_STYLE](../../com.aspose.cells/cellvalueformatstrategy\#CELL-STYLE)。

**Returns:**
int
### getIndexes() {#getIndexes--}
```
public int[] getIndexes()
```


应导出的列/行的索引。

**Returns:**
int[]
### getPlotVisibleCells() {#getPlotVisibleCells--}
```
public boolean getPlotVisibleCells()
```


仅导出可见单元格。

**Returns:**
boolean
### getPlotVisibleColumns() {#getPlotVisibleColumns--}
```
public boolean getPlotVisibleColumns()
```


仅导出可见列。

**Returns:**
boolean
### getPlotVisibleRows() {#getPlotVisibleRows--}
```
public boolean getPlotVisibleRows()
```


仅导出可见行。

**Returns:**
boolean
### getRenameStrategy() {#getRenameStrategy--}
```
public int getRenameStrategy()
```


列重复名称的策略。

请参阅 [RenameStrategy](../../com.aspose.cells/renamestrategy)。

**Returns:**
int
### getSkipErrorValue() {#getSkipErrorValue--}
```
public boolean getSkipErrorValue()
```


指示是否跳过列的无效值。例如，如果列类型是 decimal，值大于 decimal.MaxValue 且此属性为 true，我们将不会再次抛出异常。默认值为 false。

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isVertical() {#isVertical--}
```
public boolean isVertical()
```


如果 Workbook 文件中的行对应 DataTable 中的行，则为 True；如果 Workbook 文件中的列对应 DataTable 中的行，则为 False。

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### preprocessExportedValue(int cellRow, int cellColumn, CellValue value) {#preprocessExportedValue-int-int-com.aspose.cells.CellValue-}
```
public boolean preprocessExportedValue(int cellRow, int cellColumn, CellValue value)
```


预处理当前单元格的待导出值。

**Remarks**

行和列索引是单元格在工作表中的绝对索引，而不是导出表中的索引。用户可以在此方法的重写实现中检查当前单元格的值，如果需要将当前单元格替换为其他类型和数值，则实现应将期望的类型和值设置到 CellValue 对象并返回 true。默认情况下此方法不执行任何操作并返回 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cellRow | int | 当前单元格的行索引 |
| cellColumn | int | 单元格的列索引 |
| value | [CellValue](../../com.aspose.cells/cellvalue) | 当前单元格的值和类型 |

**Returns:**
布尔值 - 当前单元格是否已被替换为不同的类型和/或数值。
### setAllowDBNull(boolean value) {#setAllowDBNull-boolean-}
```
public void setAllowDBNull(boolean value)
```


此值指示是否允许在此表中使用 DBNull。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setCheckMixedValueType(boolean value) {#setCheckMixedValueType-boolean-}
```
public void setCheckMixedValueType(boolean value)
```


False，Aspose.Cells 将根据第一行的值类型设置 DataColumn 的类型以提升性能。True，Aspose.Cells 会在设置 DataColumn 的类型之前检查列中的值类型是否混合；如果值类型混合，DataColumn 的类型将为 string。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExportAsHtmlString(boolean value) {#setExportAsHtmlString-boolean-}
```
public void setExportAsHtmlString(boolean value)
```


将单元格的 HTML 字符串值导出到 DataTable。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExportAsString(boolean value) {#setExportAsString-boolean-}
```
public void setExportAsString(boolean value)
```


将单元格的字符串值导出到 DataTable。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExportColumnName(boolean value) {#setExportColumnName-boolean-}
```
public void setExportColumnName(boolean value)
```


指示是否将第一行的数据导出为 DataTable 的列名。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setFormatStrategy(int value) {#setFormatStrategy-int-}
```
public void setFormatStrategy(int value)
```


设置将值导出为字符串时的格式策略。

参见 [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy)。

**Remarks**

默认值是 [CellValueFormatStrategy.CELL\_STYLE](../../com.aspose.cells/cellvalueformatstrategy\#CELL-STYLE)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setIndexes(int[] value) {#setIndexes-int---}
```
public void setIndexes(int[] value)
```


应导出的列/行的索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int[] |  |

### setPlotVisibleCells(boolean value) {#setPlotVisibleCells-boolean-}
```
public void setPlotVisibleCells(boolean value)
```


仅导出可见单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setPlotVisibleColumns(boolean value) {#setPlotVisibleColumns-boolean-}
```
public void setPlotVisibleColumns(boolean value)
```


仅导出可见列。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setPlotVisibleRows(boolean value) {#setPlotVisibleRows-boolean-}
```
public void setPlotVisibleRows(boolean value)
```


仅导出可见行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setRenameStrategy(int value) {#setRenameStrategy-int-}
```
public void setRenameStrategy(int value)
```


列重复名称的策略。

请参阅 [RenameStrategy](../../com.aspose.cells/renamestrategy)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setSkipErrorValue(boolean value) {#setSkipErrorValue-boolean-}
```
public void setSkipErrorValue(boolean value)
```


指示是否跳过列的无效值。例如，如果列类型是 decimal，值大于 decimal.MaxValue 且此属性为 true，我们将不会再次抛出异常。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setVertical(boolean value) {#setVertical-boolean-}
```
public void setVertical(boolean value)
```


如果 Workbook 文件中的行对应 DataTable 中的行，则为 True；如果 Workbook 文件中的列对应 DataTable 中的行，则为 False。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

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

