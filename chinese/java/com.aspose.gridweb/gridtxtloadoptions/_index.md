---
title: "GridTxtLoadOptions"
second_title: "Aspose.Cells for Java API 参考"
description: "表示加载文本文件的选项。"
type: docs
url: /zh/java/com.aspose.gridweb/gridtxtloadoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.GridLoadOptions](../../com.aspose.gridweb/gridloadoptions)
```
public class GridTxtLoadOptions extends GridLoadOptions
```

表示加载文本文件的选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [GridTxtLoadOptions()](#GridTxtLoadOptions--) | 创建加载文本文件的选项。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | 指示在加载文件时是否自动过滤数据。 |
| [getCheckDataValid()](#getCheckDataValid--) | 检查模板文件中的数据是否有效。 |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | 是否在用户修改单元格相关对象时检查 Excel 文件的限制。 |
| [getClass()](#getClass--) |  |
| [getConvertDateTimeData()](#getConvertDateTimeData--) | 获取一个值，指示文本文件中的字符串是否转换为日期数据。 |
| [getConvertNumericData()](#getConvertNumericData--) | 获取一个值，指示文本文件中的字符串是否转换为数值数据。 |
| [getEncoding()](#getEncoding--) | 获取默认编码。 |
| [getExtendToNextSheet()](#getExtendToNextSheet--) | 当数据的行或列超出限制时，是否将数据扩展到下一张工作表。 |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--) | 忽略直接打印文件时未打印的数据 |
| [getKeepPrecision()](#getKeepPrecision--) | 指示当字符串长度为 15 时是否不解析该字符串值。 |
| [getKeepUnparsedData()](#getKeepUnparsedData--) | 是否在从模板文件加载工作簿时将未解析的数据保留在内存中。 |
| [getOnlyAuto()](#getOnlyAuto--) | 指示是否仅适配高度未自定义的行。 |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | 指示在读取文件时是否解析公式。 |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--) | 指示在加载文件时是否解析数据透视表缓存记录。 |
| [getPassword()](#getPassword--) | 获取工作簿的密码。 |
| [getPreservePaddingSpacesInFormula()](#getPreservePaddingSpacesInFormula--) | 指示在获取和设置公式时是否保留公式标记之间填充的空格和换行符。 |
| [getSeparator()](#getSeparator--) | 获取文本文件的字符分隔符。 |
| [getSeparatorString()](#getSeparatorString--) | 获取字符串值作为分隔符。 |
| [getTextQualifier()](#getTextQualifier--) | 指定单元格值的文本限定符。 |
| [getTreatConsecutiveDelimitersAsOne()](#getTreatConsecutiveDelimitersAsOne--) | 是否应将连续的分隔符视为一个。 |
| [getTreatQuotePrefixAsValue()](#getTreatQuotePrefixAsValue--) | 指示是否应将前导单引号视为单元格值的一部分。 |
| [hasFormula()](#hasFormula--) | 指示如果文本以 "=" 开头，则是否为公式。 |
| [hasTextQualifier()](#hasTextQualifier--) | 是否存在单元格值的文本限定符。 |
| [hashCode()](#hashCode--) |  |
| [isMultiEncoded()](#isMultiEncoded--) | True 表示文件包含多种编码。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFilter(boolean value)](#setAutoFilter-boolean-) | 指示在加载文件时是否自动过滤数据。 |
| [setCheckDataValid(boolean value)](#setCheckDataValid-boolean-) | 检查模板文件中的数据是否有效。 |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | 是否在用户修改单元格相关对象时检查 Excel 文件的限制。 |
| [setConvertDateTimeData(boolean value)](#setConvertDateTimeData-boolean-) | 设置一个值，指示文本文件中的字符串是否转换为日期数据。 |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | 设置一个值，指示文本文件中的字符串是否转换为数值数据。 |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.gridweb.Encoding-) | 设置默认编码。 |
| [setExtendToNextSheet(boolean value)](#setExtendToNextSheet-boolean-) | 当数据的行或列超出限制时，是否将数据扩展到下一张工作表。 |
| [setHasFormula(boolean value)](#setHasFormula-boolean-) | 指示如果文本以 "=" 开头，则是否为公式。 |
| [setHasTextQualifier(boolean value)](#setHasTextQualifier-boolean-) | 是否存在单元格值的文本限定符。 |
| [setIgnoreNotPrinted(boolean value)](#setIgnoreNotPrinted-boolean-) | 忽略直接打印文件时未打印的数据 |
| [setKeepPrecision(boolean value)](#setKeepPrecision-boolean-) | 指示当字符串长度为 15 时是否不解析该字符串值。 |
| [setKeepUnparsedData(boolean value)](#setKeepUnparsedData-boolean-) | 是否在从模板文件加载工作簿时将未解析的数据保留在内存中。 |
| [setMultiEncoded(boolean value)](#setMultiEncoded-boolean-) | True 表示文件包含多种编码。 |
| [setOnlyAuto(boolean value)](#setOnlyAuto-boolean-) | 指示是否仅适配高度未自定义的行。 |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | 指示在读取文件时是否解析公式。 |
| [setParsingPivotCachedRecords(boolean value)](#setParsingPivotCachedRecords-boolean-) | 指示在加载文件时是否解析数据透视表缓存记录。 |
| [setPassword(String value)](#setPassword-java.lang.String-) | 设置工作簿的密码。 |
| [setPreservePaddingSpacesInFormula(boolean value)](#setPreservePaddingSpacesInFormula-boolean-) | 指示在获取和设置公式时是否保留公式标记之间填充的空格和换行符。 |
| [setSeparator(char value)](#setSeparator-char-) | 设置文本文件的字符分隔符。 |
| [setSeparatorString(String value)](#setSeparatorString-java.lang.String-) | 设置字符串值作为分隔符。 |
| [setTextQualifier(char value)](#setTextQualifier-char-) | 指定单元格值的文本限定符。 |
| [setTreatConsecutiveDelimitersAsOne(boolean value)](#setTreatConsecutiveDelimitersAsOne-boolean-) | 是否应将连续的分隔符视为一个。 |
| [setTreatQuotePrefixAsValue(boolean value)](#setTreatQuotePrefixAsValue-boolean-) | 指示是否应将前导单引号视为单元格值的一部分。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridTxtLoadOptions() {#GridTxtLoadOptions--}
```
public GridTxtLoadOptions()
```


创建加载文本文件的选项。

**Remarks**

默认加载文件类型为 CSV。

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
### getConvertDateTimeData() {#getConvertDateTimeData--}
```
public boolean getConvertDateTimeData()
```


获取一个值，指示文本文件中的字符串是否转换为日期数据。

**Returns:**
boolean
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```


获取一个值，指示文本文件中的字符串是否转换为数值数据。

**Returns:**
boolean
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


获取默认编码。仅适用于 csv 文件。

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding)
### getExtendToNextSheet() {#getExtendToNextSheet--}
```
public boolean getExtendToNextSheet()
```


当数据的行或列超出限制时，是否将数据扩展到下一工作表。如果此属性为 true，额外的数据将扩展到当前工作表之后的下一工作表（如果当前工作表是最后一个，则会在当前工作簿中追加新工作表）。如果此属性为 false，超出限制的数据将被忽略。默认值为 false；

**Returns:**
boolean
### getIgnoreNotPrinted() {#getIgnoreNotPrinted--}
```
public boolean getIgnoreNotPrinted()
```


忽略直接打印文件时未打印的数据

**Remarks**

仅适用于 xlsx 文件。

**Returns:**
boolean
### getKeepPrecision() {#getKeepPrecision--}
```
public boolean getKeepPrecision()
```


指示当字符串长度为 15 时是否不解析该字符串值。

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
### getSeparator() {#getSeparator--}
```
public char getSeparator()
```


获取文本文件的字符分隔符。

**Returns:**
char
### getSeparatorString() {#getSeparatorString--}
```
public String getSeparatorString()
```


获取字符串值作为分隔符。

**Returns:**
java.lang.String
### getTextQualifier() {#getTextQualifier--}
```
public char getTextQualifier()
```


指定单元格值的文本限定符。默认限定符为 '"'。

**Remarks**

设置此属性时，[hasTextQualifier()](../../com.aspose.gridweb/gridtxtloadoptions\#hasTextQualifier--) 将自动变为 true。

**Returns:**
char
### getTreatConsecutiveDelimitersAsOne() {#getTreatConsecutiveDelimitersAsOne--}
```
public boolean getTreatConsecutiveDelimitersAsOne()
```


是否应将连续的分隔符视为一个。

**Returns:**
boolean
### getTreatQuotePrefixAsValue() {#getTreatQuotePrefixAsValue--}
```
public boolean getTreatQuotePrefixAsValue()
```


指示是否应将前导单引号视为单元格值的一部分。默认值为 true。如果为 false，前导单引号将从相应单元格的值中移除，并且 [GridTableItemStyle.getQuotePrefix()](../../com.aspose.gridweb/gridtableitemstyle\#getQuotePrefix--) 将被设为 true。

**Returns:**
boolean
### hasFormula() {#hasFormula--}
```
public boolean hasFormula()
```


指示如果文本以 "=" 开头，则是否为公式。

**Returns:**
boolean
### hasTextQualifier() {#hasTextQualifier--}
```
public boolean hasTextQualifier()
```


是否存在单元格值的文本限定符。默认值为 true。

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isMultiEncoded() {#isMultiEncoded--}
```
public boolean isMultiEncoded()
```


True 表示文件包含多种编码。

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

### setConvertDateTimeData(boolean value) {#setConvertDateTimeData-boolean-}
```
public void setConvertDateTimeData(boolean value)
```


设置一个值，指示文本文件中的字符串是否转换为日期数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


设置一个值，指示文本文件中的字符串是否转换为数值数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.gridweb.Encoding-}
```
public void setEncoding(Encoding value)
```


设置默认编码。仅适用于 csv 文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.gridweb/encoding) |  |

### setExtendToNextSheet(boolean value) {#setExtendToNextSheet-boolean-}
```
public void setExtendToNextSheet(boolean value)
```


当数据的行或列超出限制时，是否将数据扩展到下一工作表。如果此属性为 true，额外的数据将扩展到当前工作表之后的下一工作表（如果当前工作表是最后一个，则会在当前工作簿中追加新工作表）。如果此属性为 false，超出限制的数据将被忽略。默认值为 false；

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setHasFormula(boolean value) {#setHasFormula-boolean-}
```
public void setHasFormula(boolean value)
```


指示如果文本以 "=" 开头，则是否为公式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setHasTextQualifier(boolean value) {#setHasTextQualifier-boolean-}
```
public void setHasTextQualifier(boolean value)
```


是否存在单元格值的文本限定符。默认值为 true。

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

### setKeepPrecision(boolean value) {#setKeepPrecision-boolean-}
```
public void setKeepPrecision(boolean value)
```


指示当字符串长度为 15 时是否不解析该字符串值。

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

### setMultiEncoded(boolean value) {#setMultiEncoded-boolean-}
```
public void setMultiEncoded(boolean value)
```


True 表示文件包含多种编码。

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

### setSeparator(char value) {#setSeparator-char-}
```
public void setSeparator(char value)
```


设置文本文件的字符分隔符。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | char |  |

### setSeparatorString(String value) {#setSeparatorString-java.lang.String-}
```
public void setSeparatorString(String value)
```


设置字符串值作为分隔符。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setTextQualifier(char value) {#setTextQualifier-char-}
```
public void setTextQualifier(char value)
```


指定单元格值的文本限定符。默认限定符为 '"'。

**Remarks**

设置此属性时，[hasTextQualifier()](../../com.aspose.gridweb/gridtxtloadoptions\#hasTextQualifier--) 将自动变为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | char |  |

### setTreatConsecutiveDelimitersAsOne(boolean value) {#setTreatConsecutiveDelimitersAsOne-boolean-}
```
public void setTreatConsecutiveDelimitersAsOne(boolean value)
```


是否应将连续的分隔符视为一个。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setTreatQuotePrefixAsValue(boolean value) {#setTreatQuotePrefixAsValue-boolean-}
```
public void setTreatQuotePrefixAsValue(boolean value)
```


指示是否应将前导单引号视为单元格值的一部分。默认值为 true。如果为 false，前导单引号将从相应单元格的值中移除，并且 [GridTableItemStyle.getQuotePrefix()](../../com.aspose.gridweb/gridtableitemstyle\#getQuotePrefix--) 将被设为 true。

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

