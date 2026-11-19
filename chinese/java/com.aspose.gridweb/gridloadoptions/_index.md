---
title: "GridLoadOptions"
second_title: "Aspose.Cells for Java API 参考"
description: "表示加载文件的选项。"
type: docs
url: /zh/java/com.aspose.gridweb/gridloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class GridLoadOptions
```

表示加载文件的选项。 [Obsolete(\"This class will be obsoleted after stand alone dll usage of cells public api,instead you can use Aspose.Cells.LodOptions \")]
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [GridLoadOptions()](#GridLoadOptions--) | 创建加载文件的选项。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | 指示在加载文件时是否自动过滤数据。 |
| [getCheckDataValid()](#getCheckDataValid--) | 检查模板文件中的数据是否有效。 |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | 是否在用户修改单元格相关对象时检查 Excel 文件的限制。 |
| [getClass()](#getClass--) |  |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--) | 忽略直接打印文件时未打印的数据 |
| [getKeepUnparsedData()](#getKeepUnparsedData--) | 是否在从模板文件加载工作簿时将未解析的数据保留在内存中。 |
| [getOnlyAuto()](#getOnlyAuto--) | 指示是否仅适配高度未自定义的行。 |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | 指示在读取文件时是否解析公式。 |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--) | 指示在加载文件时是否解析数据透视表缓存记录。 |
| [getPassword()](#getPassword--) | 获取工作簿的密码。 |
| [getPreservePaddingSpacesInFormula()](#getPreservePaddingSpacesInFormula--) | 指示在获取和设置公式时是否保留公式标记之间填充的空格和换行符。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFilter(boolean value)](#setAutoFilter-boolean-) | 指示在加载文件时是否自动过滤数据。 |
| [setCheckDataValid(boolean value)](#setCheckDataValid-boolean-) | 检查模板文件中的数据是否有效。 |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | 是否在用户修改单元格相关对象时检查 Excel 文件的限制。 |
| [setIgnoreNotPrinted(boolean value)](#setIgnoreNotPrinted-boolean-) | 忽略直接打印文件时未打印的数据 |
| [setKeepUnparsedData(boolean value)](#setKeepUnparsedData-boolean-) | 是否在从模板文件加载工作簿时将未解析的数据保留在内存中。 |
| [setOnlyAuto(boolean value)](#setOnlyAuto-boolean-) | 指示是否仅适配高度未自定义的行。 |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | 指示在读取文件时是否解析公式。 |
| [setParsingPivotCachedRecords(boolean value)](#setParsingPivotCachedRecords-boolean-) | 指示在加载文件时是否解析数据透视表缓存记录。 |
| [setPassword(String value)](#setPassword-java.lang.String-) | 设置工作簿的密码。 |
| [setPreservePaddingSpacesInFormula(boolean value)](#setPreservePaddingSpacesInFormula-boolean-) | 指示在获取和设置公式时是否保留公式标记之间填充的空格和换行符。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridLoadOptions() {#GridLoadOptions--}
```
public GridLoadOptions()
```


创建加载文件的选项。

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
### getAutoFilter() {#getAutoFilter--}
```
public boolean getAutoFilter()
```


指示在加载文件时是否自动过滤数据。

**Remarks**

有时即使已设置自动筛选，文件中相应的行仍未隐藏。现在仅适用于 SpreadSheetML 文件。

**Returns:**
boolean
### getCheckDataValid() {#getCheckDataValid--}
```
public boolean getCheckDataValid()
```


检查模板文件中的数据是否有效。

**Returns:**
boolean
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


是否在用户修改单元格相关对象时检查 Excel 文件的限制。例如，Excel 不允许输入超过 32K 的字符串值。当您通过 Cell.PutValue(string) 输入超过 32K 的值时，如果此属性为 true，您将收到异常；如果此属性为 false，我们将接受您的输入字符串作为单元格的值，以便稍后能够将完整的字符串值输出为 CSV 等其他文件格式。然而，如果您设置了对 Excel 文件格式无效的此类值，之后不应将工作簿保存为 Excel 文件格式，否则生成的 Excel 文件可能会出现意外错误。

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getIgnoreNotPrinted() {#getIgnoreNotPrinted--}
```
public boolean getIgnoreNotPrinted()
```


忽略直接打印文件时未打印的数据

**Remarks**

仅适用于 xlsx 文件。

**Returns:**
boolean
### getKeepUnparsedData() {#getKeepUnparsedData--}
```
public boolean getKeepUnparsedData()
```


是否在从模板文件加载工作簿时在内存中保留未解析的数据。默认值为 true。

**Remarks**

对于仅需要从模板文件读取部分内容且不需要将工作簿保存回去的场景，将此属性设为 false 可以提升性能，尤其是在与某种 LoadFilter 一起使用时，

**Returns:**
boolean
### getOnlyAuto() {#getOnlyAuto--}
```
public boolean getOnlyAuto()
```


指示是否仅适配高度未自定义的行。

**Returns:**
boolean
### getParsingFormulaOnOpen() {#getParsingFormulaOnOpen--}
```
public boolean getParsingFormulaOnOpen()
```


指示在读取文件时是否解析公式。

**Remarks**

仅适用于 Excel Xlsx、Xltx、Xltm 和 Xlsm 文件，因为这些文件中的公式以字符串形式存储。

**Returns:**
boolean
### getParsingPivotCachedRecords() {#getParsingPivotCachedRecords--}
```
public boolean getParsingPivotCachedRecords()
```


指示在加载文件时是否解析数据透视表的缓存记录。默认值为 false。

**Remarks**

仅适用于 Excel Xlsx、Xltx、Xltm、Xlsm 和 xlsb 文件

**Returns:**
boolean
### getPassword() {#getPassword--}
```
public String getPassword()
```


获取工作簿的密码。

**Returns:**
java.lang.String
### getPreservePaddingSpacesInFormula() {#getPreservePaddingSpacesInFormula--}
```
public boolean getPreservePaddingSpacesInFormula()
```


指示在获取和设置公式时是否保留公式标记之间填充的空格和换行。默认值为 false。

**Remarks**

使用此选项从模板文件加载工作簿后，[GridWorkbookSettings.getPreservePaddingSpaces()](../../com.aspose.gridweb/gridworkbooksettings\\#getPreservePaddingSpaces--) 将被设置为与此属性相同的值。

**Returns:**
boolean
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




### setAutoFilter(boolean value) {#setAutoFilter-boolean-}
```
public void setAutoFilter(boolean value)
```


指示在加载文件时是否自动过滤数据。

**Remarks**

有时即使已设置自动筛选，文件中相应的行仍未隐藏。现在仅适用于 SpreadSheetML 文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setCheckDataValid(boolean value) {#setCheckDataValid-boolean-}
```
public void setCheckDataValid(boolean value)
```


检查模板文件中的数据是否有效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


是否在用户修改单元格相关对象时检查 Excel 文件的限制。例如，Excel 不允许输入超过 32K 的字符串值。当您通过 Cell.PutValue(string) 输入超过 32K 的值时，如果此属性为 true，您将收到异常；如果此属性为 false，我们将接受您的输入字符串作为单元格的值，以便稍后能够将完整的字符串值输出为 CSV 等其他文件格式。然而，如果您设置了对 Excel 文件格式无效的此类值，之后不应将工作簿保存为 Excel 文件格式，否则生成的 Excel 文件可能会出现意外错误。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setIgnoreNotPrinted(boolean value) {#setIgnoreNotPrinted-boolean-}
```
public void setIgnoreNotPrinted(boolean value)
```


忽略直接打印文件时未打印的数据

**Remarks**

仅适用于 xlsx 文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setKeepUnparsedData(boolean value) {#setKeepUnparsedData-boolean-}
```
public void setKeepUnparsedData(boolean value)
```


是否在从模板文件加载工作簿时在内存中保留未解析的数据。默认值为 true。

**Remarks**

对于仅需要从模板文件读取部分内容且不需要将工作簿保存回去的场景，将此属性设为 false 可以提升性能，尤其是在与某种 LoadFilter 一起使用时，

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setOnlyAuto(boolean value) {#setOnlyAuto-boolean-}
```
public void setOnlyAuto(boolean value)
```


指示是否仅适配高度未自定义的行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setParsingFormulaOnOpen(boolean value) {#setParsingFormulaOnOpen-boolean-}
```
public void setParsingFormulaOnOpen(boolean value)
```


指示在读取文件时是否解析公式。

**Remarks**

仅适用于 Excel Xlsx、Xltx、Xltm 和 Xlsm 文件，因为这些文件中的公式以字符串形式存储。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setParsingPivotCachedRecords(boolean value) {#setParsingPivotCachedRecords-boolean-}
```
public void setParsingPivotCachedRecords(boolean value)
```


指示在加载文件时是否解析数据透视表的缓存记录。默认值为 false。

**Remarks**

仅适用于 Excel Xlsx、Xltx、Xltm、Xlsm 和 xlsb 文件

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


设置工作簿的密码。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setPreservePaddingSpacesInFormula(boolean value) {#setPreservePaddingSpacesInFormula-boolean-}
```
public void setPreservePaddingSpacesInFormula(boolean value)
```


指示在获取和设置公式时是否保留公式标记之间填充的空格和换行。默认值为 false。

**Remarks**

使用此选项从模板文件加载工作簿后，[GridWorkbookSettings.getPreservePaddingSpaces()](../../com.aspose.gridweb/gridworkbooksettings\\#getPreservePaddingSpaces--) 将被设置为与此属性相同的值。

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

