---
title: "ImportTableOptions"
second_title: "Aspose.Cells for Java API 参考"
description: "表示导入数据到单元格的选项。"
type: docs
url: /zh/java/com.aspose.cells/importtableoptions/
---

**Inheritance:**
java.lang.Object
```
public class ImportTableOptions
```

表示导入数据到单元格的选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [ImportTableOptions()](#ImportTableOptions--) | 创建默认的导入选项。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCheckMergedCells()](#getCheckMergedCells--) | 指示是否检查合并单元格。 |
| [getClass()](#getClass--) |  |
| [getColumnIndexes()](#getColumnIndexes--) | 获取要从数据源导入的列（基于 0 的索引）。null 表示应导入所有列。 |
| [getConvertGridStyle()](#getConvertGridStyle--) | 指示是否将网格视图的样式应用于单元格。 |
| [getConvertNumericData()](#getConvertNumericData--) | 获取一个值，指示字符串值是否应转换为数值或日期值。 |
| [getDateFormat()](#getDateFormat--) | 获取用于导入日期时间值的单元格的日期格式字符串。 |
| [getDefaultValues()](#getDefaultValues--) | 表中值的默认值为 null。 |
| [getExportCaptionAsFieldName()](#getExportCaptionAsFieldName--) | 指示是否将标题导出为字段名 |
| [getInsertRows()](#getInsertRows--) | 指示是否应为导入的数据记录添加新行。 |
| [getNumberFormats()](#getNumberFormats--) | 获取数字格式 |
| [getShiftFirstRowDown()](#getShiftFirstRowDown--) | 指示在插入行时是否将第一行向下移动。 |
| [getStyles()](#getStyles--) | 获取表中每列的样式。 |
| [getTotalColumns()](#getTotalColumns--) | 获取要从数据源导入的列总数。-1 表示给定数据源的所有列。 |
| [getTotalRows()](#getTotalRows--) | 获取要从数据源导入的行总数。-1 表示给定数据源的所有行。 |
| [hashCode()](#hashCode--) |  |
| [isFieldNameShown()](#isFieldNameShown--) | 指示是否应导入字段名。 |
| [isFormulas()](#isFormulas--) | 指示数据是否为公式。 |
| [isHtmlString()](#isHtmlString--) | 指示该值是否包含 html 标记。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCheckMergedCells(boolean value)](#setCheckMergedCells-boolean-) | 指示是否检查合并单元格。 |
| [setColumnIndexes(int[] value)](#setColumnIndexes-int---) | 设置要从数据源导入的列（基于 0 的索引）。null 表示应导入所有列。 |
| [setConvertGridStyle(boolean value)](#setConvertGridStyle-boolean-) | 指示是否将网格视图的样式应用于单元格。 |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | 设置一个值，指示字符串值是否应转换为数值或日期值。 |
| [setDateFormat(String value)](#setDateFormat-java.lang.String-) | 为导入的日期时间值的单元格设置日期格式字符串。 |
| [setDefaultValues(Object[] value)](#setDefaultValues-java.lang.Object---) | 表中值的默认值为 null。 |
| [setExportCaptionAsFieldName(boolean value)](#setExportCaptionAsFieldName-boolean-) | 指示是否将标题导出为字段名 |
| [setFieldNameShown(boolean value)](#setFieldNameShown-boolean-) | 指示是否应导入字段名。 |
| [setFormulas(boolean[] value)](#setFormulas-boolean---) | 指示数据是否为公式。 |
| [setHtmlString(boolean value)](#setHtmlString-boolean-) | 指示该值是否包含 html 标记。 |
| [setInsertRows(boolean value)](#setInsertRows-boolean-) | 指示是否应为导入的数据记录添加新行。 |
| [setNumberFormats(String[] value)](#setNumberFormats-java.lang.String---) | 设置数字格式 |
| [setShiftFirstRowDown(boolean value)](#setShiftFirstRowDown-boolean-) | 指示在插入行时是否将第一行向下移动。 |
| [setStyles(Style[] value)](#setStyles-com.aspose.cells.Style---) | 为表格的每一列设置样式。 |
| [setTotalColumns(int value)](#setTotalColumns-int-) | 设置要从数据源导入的总列数。-1 表示给定数据源的所有行。 |
| [setTotalRows(int value)](#setTotalRows-int-) | 设置要从数据源导入的总行数。-1 表示给定数据源的所有行。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ImportTableOptions() {#ImportTableOptions--}
```
public ImportTableOptions()
```


创建默认的导入选项。

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
### getCheckMergedCells() {#getCheckMergedCells--}
```
public boolean getCheckMergedCells()
```


指示是否检查合并单元格。

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnIndexes() {#getColumnIndexes--}
```
public int[] getColumnIndexes()
```


获取要从数据源导入的列（基于 0 的索引）。null 表示应导入所有列。

**Returns:**
int[]
### getConvertGridStyle() {#getConvertGridStyle--}
```
public boolean getConvertGridStyle()
```


指示是否将网格视图的样式应用于单元格。

**Returns:**
boolean
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```


获取一个值，指示字符串值是否应转换为数值或日期值。

**Returns:**
boolean
### getDateFormat() {#getDateFormat--}
```
public String getDateFormat()
```


获取用于导入日期时间值的单元格的日期格式字符串。

**Returns:**
java.lang.String
### getDefaultValues() {#getDefaultValues--}
```
public Object[] getDefaultValues()
```


表中值的默认值为 null。

**Returns:**
java.lang.Object[]
### getExportCaptionAsFieldName() {#getExportCaptionAsFieldName--}
```
public boolean getExportCaptionAsFieldName()
```


指示是否将标题导出为字段名

**Remarks**

仅适用于 DataTable。

**Returns:**
boolean
### getInsertRows() {#getInsertRows--}
```
public boolean getInsertRows()
```


指示是否应为导入的数据记录添加新行。

**Returns:**
boolean
### getNumberFormats() {#getNumberFormats--}
```
public String[] getNumberFormats()
```


获取数字格式

**Returns:**
java.lang.String[]
### getShiftFirstRowDown() {#getShiftFirstRowDown--}
```
public boolean getShiftFirstRowDown()
```


指示在插入行时是否将第一行向下移动。

**Returns:**
boolean
### getStyles() {#getStyles--}
```
public Style[] getStyles()
```


获取表中每列的样式。

**Returns:**
com.aspose.cells.Style[]
### getTotalColumns() {#getTotalColumns--}
```
public int getTotalColumns()
```


获取要从数据源导入的列总数。-1 表示给定数据源的所有列。

**Returns:**
int
### getTotalRows() {#getTotalRows--}
```
public int getTotalRows()
```


获取要从数据源导入的行总数。-1 表示给定数据源的所有行。

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isFieldNameShown() {#isFieldNameShown--}
```
public boolean isFieldNameShown()
```


指示是否应导入字段名。

**Returns:**
boolean
### isFormulas() {#isFormulas--}
```
public boolean[] isFormulas()
```


指示数据是否为公式。

**Returns:**
boolean[]
### isHtmlString() {#isHtmlString--}
```
public boolean isHtmlString()
```


指示该值是否包含 html 标记。

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




### setCheckMergedCells(boolean value) {#setCheckMergedCells-boolean-}
```
public void setCheckMergedCells(boolean value)
```


指示是否检查合并单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setColumnIndexes(int[] value) {#setColumnIndexes-int---}
```
public void setColumnIndexes(int[] value)
```


设置要从数据源导入的列（基于 0 的索引）。null 表示应导入所有列。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int[] |  |

### setConvertGridStyle(boolean value) {#setConvertGridStyle-boolean-}
```
public void setConvertGridStyle(boolean value)
```


指示是否将网格视图的样式应用于单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


设置一个值，指示字符串值是否应转换为数值或日期值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setDateFormat(String value) {#setDateFormat-java.lang.String-}
```
public void setDateFormat(String value)
```


为导入的日期时间值的单元格设置日期格式字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setDefaultValues(Object[] value) {#setDefaultValues-java.lang.Object---}
```
public void setDefaultValues(Object[] value)
```


表中值的默认值为 null。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.Object[] |  |

### setExportCaptionAsFieldName(boolean value) {#setExportCaptionAsFieldName-boolean-}
```
public void setExportCaptionAsFieldName(boolean value)
```


指示是否将标题导出为字段名

**Remarks**

仅适用于 DataTable。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setFieldNameShown(boolean value) {#setFieldNameShown-boolean-}
```
public void setFieldNameShown(boolean value)
```


指示是否应导入字段名。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setFormulas(boolean[] value) {#setFormulas-boolean---}
```
public void setFormulas(boolean[] value)
```


指示数据是否为公式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean[] |  |

### setHtmlString(boolean value) {#setHtmlString-boolean-}
```
public void setHtmlString(boolean value)
```


指示该值是否包含 html 标记。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setInsertRows(boolean value) {#setInsertRows-boolean-}
```
public void setInsertRows(boolean value)
```


指示是否应为导入的数据记录添加新行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setNumberFormats(String[] value) {#setNumberFormats-java.lang.String---}
```
public void setNumberFormats(String[] value)
```


设置数字格式

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String[] |  |

### setShiftFirstRowDown(boolean value) {#setShiftFirstRowDown-boolean-}
```
public void setShiftFirstRowDown(boolean value)
```


指示在插入行时是否将第一行向下移动。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setStyles(Style[] value) {#setStyles-com.aspose.cells.Style---}
```
public void setStyles(Style[] value)
```


为表格的每一列设置样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Style\[\]](../../com.aspose.cells/style) |  |

### setTotalColumns(int value) {#setTotalColumns-int-}
```
public void setTotalColumns(int value)
```


设置要从数据源导入的总列数。-1 表示给定数据源的所有行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTotalRows(int value) {#setTotalRows-int-}
```
public void setTotalRows(int value)
```


设置要从数据源导入的总行数。-1 表示给定数据源的所有行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

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

