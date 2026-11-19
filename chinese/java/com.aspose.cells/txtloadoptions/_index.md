---
title: "TxtLoadOptions"
second_title: "Aspose.Cells for Java API 参考"
description: "表示加载文本文件的选项。"
type: docs
url: /zh/java/com.aspose.cells/txtloadoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LoadOptions](../../com.aspose.cells/loadoptions), [com.aspose.cells.AbstractTextLoadOptions](../../com.aspose.cells/abstracttextloadoptions)
```
public class TxtLoadOptions extends AbstractTextLoadOptions
```

表示加载文本文件的选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [TxtLoadOptions()](#TxtLoadOptions--) | 创建加载文本文件的选项。 |
| [TxtLoadOptions(int loadFormat)](#TxtLoadOptions-int-) | 创建加载文本文件的选项。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | 指示在加载文件时是否自动过滤数据。 |
| [getAutoFitterOptions()](#getAutoFitterOptions--) | 获取自动适配选项 |
| [getCheckDataValid()](#getCheckDataValid--) | 检查模板文件中的数据是否有效。 |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | 是否在用户修改单元格相关对象时检查 Excel 文件的限制。 |
| [getClass()](#getClass--) |  |
| [getConvertDateTimeData()](#getConvertDateTimeData--) | 获取一个值，指示文本文件中的字符串是否转换为日期数据。 |
| [getConvertNumericData()](#getConvertNumericData--) | 获取一个值，指示文本文件中的字符串是否转换为数值数据。 |
| [getDefaultStyleSettings()](#getDefaultStyleSettings--) | 获取用于初始化工作簿样式的默认样式设置 |
| [getEncoding()](#getEncoding--) | 获取默认编码。 |
| [getExtendToNextSheet()](#getExtendToNextSheet--) | 当数据的行或列超出限制时，是否将数据扩展到下一张工作表。 |
| [getFontConfigs()](#getFontConfigs--) | 获取单独的字体配置。 |
| [getHeaderColumnsCount()](#getHeaderColumnsCount--) | 要在扩展工作表中重复的标题列数。 |
| [getHeaderRowsCount()](#getHeaderRowsCount--) | 要在扩展工作表中重复的标题行数。 |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--) | 忽略直接打印文件时未打印的数据 |
| [getIgnoreUselessShapes()](#getIgnoreUselessShapes--) | 指示是否忽略无用的形状。 |
| [getInterruptMonitor()](#getInterruptMonitor--) | 获取中断监视器。 |
| [getKeepPrecision()](#getKeepPrecision--) | 指示当字符串长度为 15 时是否不解析该字符串值。 |
| [getKeepUnparsedData()](#getKeepUnparsedData--) | 是否在从模板文件加载工作簿时将未解析的数据保留在内存中。 |
| [getLanguageCode()](#getLanguageCode--) | 获取基于已保存文件的 CountryCode 的工作簿版本的用户界面语言。 |
| [getLightCellsDataHandler()](#getLightCellsDataHandler--) | 读取模板文件时用于处理单元格数据的数据处理程序。 |
| [getLoadFilter()](#getLoadFilter--) | 用于指示如何加载数据的过滤器。 |
| [getLoadFormat()](#getLoadFormat--) | 获取加载格式。 |
| [getLoadStyleStrategy()](#getLoadStyleStrategy--) | 指示在将字符串值转换为数字或日期时间时，对解析值应用样式的策略。 |
| [getLocale()](#getLocale--) | 获取将要加载的工作簿使用的区域设置。 |
| [getMaxColumnCount()](#getMaxColumnCount--) | 单张工作表可导入的最大列数。 |
| [getMaxRowCount()](#getMaxRowCount--) | 每个工作表要导入的最大行数。 |
| [getMemorySetting()](#getMemorySetting--) | 获取已加载工作簿的内存模式。 |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | 指示在读取文件时是否解析公式。 |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--) | 指示在加载文件时是否解析数据透视表缓存记录。 |
| [getPassword()](#getPassword--) | 获取工作簿的密码。 |
| [getPreferredParsers()](#getPreferredParsers--) | 获取加载文本文件的首选值解析器。 |
| [getPreservePaddingSpacesInFormula()](#getPreservePaddingSpacesInFormula--) | 指示在获取和设置公式时是否保留公式标记之间填充的空格和换行符。 |
| [getRegion()](#getRegion--) | 获取将要加载的工作簿使用的区域设置。 |
| [getSeparator()](#getSeparator--) | 获取文本文件的字符分隔符。 |
| [getSeparatorString()](#getSeparatorString--) | 获取字符串值作为分隔符。 |
| [getStandardFont()](#getStandardFont--) | 设置默认标准字体名称 |
| [getStandardFontSize()](#getStandardFontSize--) | 设置默认标准字体大小。 |
| [getTextQualifier()](#getTextQualifier--) | 指定单元格值的文本限定符。 |
| [getTreatConsecutiveDelimitersAsOne()](#getTreatConsecutiveDelimitersAsOne--) | 是否应将连续的分隔符视为一个。 |
| [getTreatQuotePrefixAsValue()](#getTreatQuotePrefixAsValue--) | 指示是否应将前导单引号视为单元格值的一部分。 |
| [getWarningCallback()](#getWarningCallback--) | 获取警告回调。 |
| [hasFormula()](#hasFormula--) | 指示如果文本以 "=" 开头，则是否为公式。 |
| [hasTextQualifier()](#hasTextQualifier--) | 是否存在单元格值的文本限定符。 |
| [hashCode()](#hashCode--) |  |
| [isMultiEncoded()](#isMultiEncoded--) | True 表示文件包含多种编码。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFilter(boolean value)](#setAutoFilter-boolean-) | 指示在加载文件时是否自动过滤数据。 |
| [setAutoFitterOptions(AutoFitterOptions value)](#setAutoFitterOptions-com.aspose.cells.AutoFitterOptions-) | 设置自动适配选项 |
| [setCheckDataValid(boolean value)](#setCheckDataValid-boolean-) | 检查模板文件中的数据是否有效。 |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | 是否在用户修改单元格相关对象时检查 Excel 文件的限制。 |
| [setConvertDateTimeData(boolean value)](#setConvertDateTimeData-boolean-) | 设置一个值，指示文本文件中的字符串是否转换为日期数据。 |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | 设置一个值，指示文本文件中的字符串是否转换为数值数据。 |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | 设置默认编码。 |
| [setExtendToNextSheet(boolean value)](#setExtendToNextSheet-boolean-) | 当数据的行或列超出限制时，是否将数据扩展到下一张工作表。 |
| [setFontConfigs(IndividualFontConfigs value)](#setFontConfigs-com.aspose.cells.IndividualFontConfigs-) | 设置单个字体配置。 |
| [setHasFormula(boolean value)](#setHasFormula-boolean-) | 指示如果文本以 "=" 开头，则是否为公式。 |
| [setHasTextQualifier(boolean value)](#setHasTextQualifier-boolean-) | 是否存在单元格值的文本限定符。 |
| [setHeaderColumnsCount(int value)](#setHeaderColumnsCount-int-) | 要在扩展工作表中重复的标题列数。 |
| [setHeaderRowsCount(int value)](#setHeaderRowsCount-int-) | 要在扩展工作表中重复的标题行数。 |
| [setIgnoreNotPrinted(boolean value)](#setIgnoreNotPrinted-boolean-) | 忽略直接打印文件时未打印的数据 |
| [setIgnoreUselessShapes(boolean value)](#setIgnoreUselessShapes-boolean-) | 指示是否忽略无用的形状。 |
| [setInterruptMonitor(AbstractInterruptMonitor value)](#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-) | 设置中断监视器。 |
| [setKeepPrecision(boolean value)](#setKeepPrecision-boolean-) | 指示当字符串长度为 15 时是否不解析该字符串值。 |
| [setKeepUnparsedData(boolean value)](#setKeepUnparsedData-boolean-) | 是否在从模板文件加载工作簿时将未解析的数据保留在内存中。 |
| [setLanguageCode(int value)](#setLanguageCode-int-) | 根据保存文件的 CountryCode 设置工作簿版本的用户界面语言。 |
| [setLightCellsDataHandler(LightCellsDataHandler value)](#setLightCellsDataHandler-com.aspose.cells.LightCellsDataHandler-) | 读取模板文件时用于处理单元格数据的数据处理程序。 |
| [setLoadFilter(LoadFilter value)](#setLoadFilter-com.aspose.cells.LoadFilter-) | 用于指示如何加载数据的过滤器。 |
| [setLoadStyleStrategy(int value)](#setLoadStyleStrategy-int-) | 指示在将字符串值转换为数字或日期时间时，对解析值应用样式的策略。 |
| [setLocale(Locale value)](#setLocale-java.util.Locale-) | 设置将要加载的工作簿使用的区域设置。 |
| [setMaxColumnCount(int value)](#setMaxColumnCount-int-) | 单张工作表可导入的最大列数。 |
| [setMaxRowCount(int value)](#setMaxRowCount-int-) | 每个工作表要导入的最大行数。 |
| [setMemorySetting(int value)](#setMemorySetting-int-) | 设置已加载工作簿的内存模式。 |
| [setMultiEncoded(boolean value)](#setMultiEncoded-boolean-) | True 表示文件包含多种编码。 |
| [setPaperSize(int type)](#setPaperSize-int-) | 根据默认打印机的设置设置默认打印纸张大小。 |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | 指示在读取文件时是否解析公式。 |
| [setParsingPivotCachedRecords(boolean value)](#setParsingPivotCachedRecords-boolean-) | 指示在加载文件时是否解析数据透视表缓存记录。 |
| [setPassword(String value)](#setPassword-java.lang.String-) | 设置工作簿的密码。 |
| [setPreferredParsers(ICustomParser[] value)](#setPreferredParsers-com.aspose.cells.ICustomParser---) | 设置加载文本文件的首选值解析器。 |
| [setPreservePaddingSpacesInFormula(boolean value)](#setPreservePaddingSpacesInFormula-boolean-) | 指示在获取和设置公式时是否保留公式标记之间填充的空格和换行符。 |
| [setRegion(int value)](#setRegion-int-) | 设置将要加载的工作簿使用的区域设置。 |
| [setSeparator(char value)](#setSeparator-char-) | 设置文本文件的字符分隔符。 |
| [setSeparatorString(String value)](#setSeparatorString-java.lang.String-) | 设置字符串值作为分隔符。 |
| [setStandardFont(String value)](#setStandardFont-java.lang.String-) | 设置默认标准字体名称 |
| [setStandardFontSize(double value)](#setStandardFontSize-double-) | 设置默认标准字体大小。 |
| [setTextQualifier(char value)](#setTextQualifier-char-) | 指定单元格值的文本限定符。 |
| [setTreatConsecutiveDelimitersAsOne(boolean value)](#setTreatConsecutiveDelimitersAsOne-boolean-) | 是否应将连续的分隔符视为一个。 |
| [setTreatQuotePrefixAsValue(boolean value)](#setTreatQuotePrefixAsValue-boolean-) | 指示是否应将前导单引号视为单元格值的一部分。 |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | 设置警告回调。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### TxtLoadOptions() {#TxtLoadOptions--}
```
public TxtLoadOptions()
```


创建加载文本文件的选项。

**Remarks**

默认加载文件类型为 CSV。

### TxtLoadOptions(int loadFormat) {#TxtLoadOptions-int-}
```
public TxtLoadOptions(int loadFormat)
```


创建加载文本文件的选项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| loadFormat | int | [LoadFormat](../../com.aspose.cells/loadformat)。加载格式 |

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
### getAutoFitterOptions() {#getAutoFitterOptions--}
```
public AutoFitterOptions getAutoFitterOptions()
```


获取自动适配选项

**Remarks**

仅适用于 xlsx、spreadsheetML 文件。

**Returns:**
[AutoFitterOptions](../../com.aspose.cells/autofitteroptions)
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


获取一个值，指示文本文件中的字符串是否转换为日期数据。默认值为 true。

**Returns:**
boolean
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```


获取一个值，指示文本文件中的字符串是否转换为数值数据。默认值为 true。

**Returns:**
boolean
### getDefaultStyleSettings() {#getDefaultStyleSettings--}
```
public DefaultStyleSettings getDefaultStyleSettings()
```


获取用于初始化工作簿样式的默认样式设置

**Returns:**
[DefaultStyleSettings](../../com.aspose.cells/defaultstylesettings)
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


获取默认编码。仅适用于 csv 文件。

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getExtendToNextSheet() {#getExtendToNextSheet--}
```
public boolean getExtendToNextSheet()
```


当数据的行或列超出限制时，是否将数据扩展到下一个工作表。默认值为 false。

**Remarks**

如果此属性为 true，额外数据将放入当前工作表后面的下一个工作表（如果当前工作表是最后一个，则在当前工作簿中追加新工作表）。如果此属性为 false，超出限制的数据将被忽略。

**Returns:**
boolean
### getFontConfigs() {#getFontConfigs--}
```
public IndividualFontConfigs getFontConfigs()
```


获取单个字体配置。仅适用于使用此 [LoadOptions](../../com.aspose.cells/loadoptions) 加载的 [Workbook](../../com.aspose.cells/workbook)。

**Returns:**
[IndividualFontConfigs](../../com.aspose.cells/individualfontconfigs)
### getHeaderColumnsCount() {#getHeaderColumnsCount--}
```
public int getHeaderColumnsCount()
```


要在扩展工作表中重复的标题列数。

**Remarks**

此属性指定的标题列将在那些扩展的工作表中复制。仅当 [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\\#getExtendToNextSheet--) 为 true 时，此属性才生效。

**Returns:**
int
### getHeaderRowsCount() {#getHeaderRowsCount--}
```
public int getHeaderRowsCount()
```


要在扩展工作表中重复的标题行数。

**Remarks**

此属性指定的标题行将在那些扩展的工作表中复制。仅当 [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\\#getExtendToNextSheet--) 为 true 时，此属性才生效。

**Returns:**
int
### getIgnoreNotPrinted() {#getIgnoreNotPrinted--}
```
public boolean getIgnoreNotPrinted()
```


忽略直接打印文件时未打印的数据

**Remarks**

仅适用于 xlsx 文件。

**Returns:**
boolean
### getIgnoreUselessShapes() {#getIgnoreUselessShapes--}
```
public boolean getIgnoreUselessShapes()
```


指示是否忽略无用的形状。

**Remarks**

仅适用于 xlsx、xlsb 和 xlsm 文件。某些文件中存在许多重叠的相同形状，这些形状是无用的，我们可以在加载文件时忽略它们。

**Returns:**
boolean
### getInterruptMonitor() {#getInterruptMonitor--}
```
public AbstractInterruptMonitor getInterruptMonitor()
```


获取中断监视器。

**Returns:**
[AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor)
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
### getLanguageCode() {#getLanguageCode--}
```
public int getLanguageCode()
```


获取基于已保存文件的 CountryCode 的工作簿版本的用户界面语言。

参见 [CountryCode](../../com.aspose.cells/countrycode)。

**Returns:**
int
### getLightCellsDataHandler() {#getLightCellsDataHandler--}
```
public LightCellsDataHandler getLightCellsDataHandler()
```


读取模板文件时用于处理单元格数据的数据处理程序。

**Returns:**
[LightCellsDataHandler](../../com.aspose.cells/lightcellsdatahandler)
### getLoadFilter() {#getLoadFilter--}
```
public LoadFilter getLoadFilter()
```


用于指示如何加载数据的过滤器。

**Returns:**
[LoadFilter](../../com.aspose.cells/loadfilter)
### getLoadFormat() {#getLoadFormat--}
```
public int getLoadFormat()
```


获取加载格式。

参见 [LoadFormat](../../com.aspose.cells/loadformat)。

**Returns:**
int
### getLoadStyleStrategy() {#getLoadStyleStrategy--}
```
public int getLoadStyleStrategy()
```


指示在将字符串值转换为数字或日期时间时，对解析值应用样式的策略。

参见 [TxtLoadStyleStrategy](../../com.aspose.cells/txtloadstylestrategy)。

**Returns:**
int
### getLocale() {#getLocale--}
```
public Locale getLocale()
```


获取将要加载的工作簿使用的区域设置。

**Remarks**

此属性在设置区域设置时具有与 [getRegion()](../../com.aspose.cells/loadoptions\#getRegion--) 相同的效果。

**Returns:**
java.util.Locale
### getMaxColumnCount() {#getMaxColumnCount--}
```
public int getMaxColumnCount()
```


单张工作表可导入的最大列数。

**Remarks**

超过此限制的列将根据 [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\\#getExtendToNextSheet--) 被忽略或扩展到下一个工作表。此计数包括标题列（[getHeaderColumnsCount()](../../com.aspose.cells/txtloadoptions\\#getHeaderColumnsCount--)）。其最大值为相应文件格式的列限制，例如 xlsx 文件为 16384。如果未指定此属性或指定的值不是正数，则也将使用最大限制。

**Returns:**
int
### getMaxRowCount() {#getMaxRowCount--}
```
public int getMaxRowCount()
```


每个工作表要导入的最大行数。

**Remarks**

超过此限制的行将根据 [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\\#getExtendToNextSheet--) 被忽略或扩展到下一个工作表。此计数包括标题行（[getHeaderRowsCount()](../../com.aspose.cells/txtloadoptions\\#getHeaderRowsCount--)）。其最大允许值为相应文件格式的行限制，例如 xlsx 文件为 1048576。如果未指定此属性或指定的值不是正数，则也将使用最大限制。

**Returns:**
int
### getMemorySetting() {#getMemorySetting--}
```
public int getMemorySetting()
```


获取已加载工作簿的内存模式。

参见 [MemorySetting](../../com.aspose.cells/memorysetting)。

**Remarks**

有关内存模式的更多详细信息，请参见 [Cells.getMemorySetting()](../../com.aspose.cells/cells\#getMemorySetting--)。

**Returns:**
int
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
### getPreferredParsers() {#getPreferredParsers--}
```
public ICustomParser[] getPreferredParsers()
```


获取加载文本文件的首选值解析器。

**Remarks**

parsers[0] 是用于文本模板文件第一列的解析器，parsers[1] 是用于第二列的解析器，...等。最后一个（parsers[parsers.length-1]）将用于从 parsers.length-1 开始的所有其他列。如果某个项为 null，则相应列将使用 Aspose.Cells 的默认解析器进行解析。

**Returns:**
com.aspose.cells.ICustomParser[]
### getPreservePaddingSpacesInFormula() {#getPreservePaddingSpacesInFormula--}
```
public boolean getPreservePaddingSpacesInFormula()
```


指示在获取和设置公式时是否保留公式标记之间填充的空格和换行。默认值为 false。

**Remarks**

使用此选项从模板文件加载工作簿后，[FormulaSettings.getPreservePaddingSpaces()](../../com.aspose.cells/formulasettings\#getPreservePaddingSpaces--) 将被设置为与此属性相同的值。

**Returns:**
boolean
### getRegion() {#getRegion--}
```
public int getRegion()
```


获取将要加载的工作簿使用的区域设置。

参见 [CountryCode](../../com.aspose.cells/countrycode)。

**Remarks**

区域设置可用于初始化工作簿的一些功能，例如字体、主题等。对于基于文本的文件格式，如 CSV、HTML 等，区域设置还将用于检测数字格式并将文本值解析为单元格的数值或日期时间值。此设置将在后续实例化的工作簿中保留，即工作簿的 [WorkbookSettings.getRegion()](../../com.aspose.cells/workbooksettings\#getRegion--) 将使用与此属性相同的区域。

**Returns:**
int
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
### getStandardFont() {#getStandardFont--}
```
public String getStandardFont()
```


设置默认标准字体名称

**Remarks**

注意：此成员现已过时。请改用 DefaultStyleSettings。此属性将在自 2022 年 3 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
java.lang.String
### getStandardFontSize() {#getStandardFontSize--}
```
public double getStandardFontSize()
```


设置默认标准字体大小。

**Remarks**

注意：此成员现已过时。请改用 DefaultStyleSettings。此属性将在自 2022 年 3 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
double
### getTextQualifier() {#getTextQualifier--}
```
public char getTextQualifier()
```


指定单元格值的文本限定符。默认限定符为 '"'。

**Remarks**

设置此属性时，[hasTextQualifier()](../../com.aspose.cells/txtloadoptions\\#hasTextQualifier--) 将自动变为 true。

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


指示是否应将前导单引号视为单元格值的一部分。默认值为 true。如果为 false，前导单引号将从相应单元格的值中移除，并且 [Style.getQuotePrefix()](../../com.aspose.cells/style\\#getQuotePrefix--) 将被设置为 true。

**Returns:**
boolean
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


获取警告回调。

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
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

### setAutoFitterOptions(AutoFitterOptions value) {#setAutoFitterOptions-com.aspose.cells.AutoFitterOptions-}
```
public void setAutoFitterOptions(AutoFitterOptions value)
```


设置自动适配选项

**Remarks**

仅适用于 xlsx、spreadsheetML 文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) |  |

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


设置一个值，指示文本文件中的字符串是否转换为日期数据。默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


设置一个值，指示文本文件中的字符串是否转换为数值数据。默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```


设置默认编码。仅适用于 csv 文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setExtendToNextSheet(boolean value) {#setExtendToNextSheet-boolean-}
```
public void setExtendToNextSheet(boolean value)
```


当数据的行或列超出限制时，是否将数据扩展到下一个工作表。默认值为 false。

**Remarks**

如果此属性为 true，额外数据将放入当前工作表后面的下一个工作表（如果当前工作表是最后一个，则在当前工作簿中追加新工作表）。如果此属性为 false，超出限制的数据将被忽略。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setFontConfigs(IndividualFontConfigs value) {#setFontConfigs-com.aspose.cells.IndividualFontConfigs-}
```
public void setFontConfigs(IndividualFontConfigs value)
```


设置各个字体配置。仅适用于使用此 [LoadOptions](../../com.aspose.cells/loadoptions) 加载的 [Workbook](../../com.aspose.cells/workbook)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [IndividualFontConfigs](../../com.aspose.cells/individualfontconfigs) |  |

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

### setHeaderColumnsCount(int value) {#setHeaderColumnsCount-int-}
```
public void setHeaderColumnsCount(int value)
```


要在扩展工作表中重复的标题列数。

**Remarks**

此属性指定的标题列将在那些扩展的工作表中复制。仅当 [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\\#getExtendToNextSheet--) 为 true 时，此属性才生效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setHeaderRowsCount(int value) {#setHeaderRowsCount-int-}
```
public void setHeaderRowsCount(int value)
```


要在扩展工作表中重复的标题行数。

**Remarks**

此属性指定的标题行将在那些扩展的工作表中复制。仅当 [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\\#getExtendToNextSheet--) 为 true 时，此属性才生效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

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

### setIgnoreUselessShapes(boolean value) {#setIgnoreUselessShapes-boolean-}
```
public void setIgnoreUselessShapes(boolean value)
```


指示是否忽略无用的形状。

**Remarks**

仅适用于 xlsx、xlsb 和 xlsm 文件。某些文件中存在许多重叠的相同形状，这些形状是无用的，我们可以在加载文件时忽略它们。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setInterruptMonitor(AbstractInterruptMonitor value) {#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-}
```
public void setInterruptMonitor(AbstractInterruptMonitor value)
```


设置中断监视器。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor) |  |

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

### setLanguageCode(int value) {#setLanguageCode-int-}
```
public void setLanguageCode(int value)
```


根据保存文件的 CountryCode 设置工作簿版本的用户界面语言。

参见 [CountryCode](../../com.aspose.cells/countrycode)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setLightCellsDataHandler(LightCellsDataHandler value) {#setLightCellsDataHandler-com.aspose.cells.LightCellsDataHandler-}
```
public void setLightCellsDataHandler(LightCellsDataHandler value)
```


读取模板文件时用于处理单元格数据的数据处理程序。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [LightCellsDataHandler](../../com.aspose.cells/lightcellsdatahandler) |  |

### setLoadFilter(LoadFilter value) {#setLoadFilter-com.aspose.cells.LoadFilter-}
```
public void setLoadFilter(LoadFilter value)
```


用于指示如何加载数据的过滤器。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [LoadFilter](../../com.aspose.cells/loadfilter) |  |

### setLoadStyleStrategy(int value) {#setLoadStyleStrategy-int-}
```
public void setLoadStyleStrategy(int value)
```


指示在将字符串值转换为数字或日期时间时，对解析值应用样式的策略。

参见 [TxtLoadStyleStrategy](../../com.aspose.cells/txtloadstylestrategy)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setLocale(Locale value) {#setLocale-java.util.Locale-}
```
public void setLocale(Locale value)
```


设置将要加载的工作簿使用的区域设置。

**Remarks**

此属性在设置区域设置时具有与 [getRegion()](../../com.aspose.cells/loadoptions\#getRegion--) 相同的效果。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Locale |  |

### setMaxColumnCount(int value) {#setMaxColumnCount-int-}
```
public void setMaxColumnCount(int value)
```


单张工作表可导入的最大列数。

**Remarks**

超过此限制的列将根据 [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\\#getExtendToNextSheet--) 被忽略或扩展到下一个工作表。此计数包括标题列（[getHeaderColumnsCount()](../../com.aspose.cells/txtloadoptions\\#getHeaderColumnsCount--)）。其最大值为相应文件格式的列限制，例如 xlsx 文件为 16384。如果未指定此属性或指定的值不是正数，则也将使用最大限制。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setMaxRowCount(int value) {#setMaxRowCount-int-}
```
public void setMaxRowCount(int value)
```


每个工作表要导入的最大行数。

**Remarks**

超过此限制的行将根据 [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\\#getExtendToNextSheet--) 被忽略或扩展到下一个工作表。此计数包括标题行（[getHeaderRowsCount()](../../com.aspose.cells/txtloadoptions\\#getHeaderRowsCount--)）。其最大允许值为相应文件格式的行限制，例如 xlsx 文件为 1048576。如果未指定此属性或指定的值不是正数，则也将使用最大限制。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setMemorySetting(int value) {#setMemorySetting-int-}
```
public void setMemorySetting(int value)
```


设置已加载工作簿的内存模式。

参见 [MemorySetting](../../com.aspose.cells/memorysetting)。

**Remarks**

有关内存模式的更多详细信息，请参见 [Cells.getMemorySetting()](../../com.aspose.cells/cells\#getMemorySetting--)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setMultiEncoded(boolean value) {#setMultiEncoded-boolean-}
```
public void setMultiEncoded(boolean value)
```


True 表示文件包含多种编码。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setPaperSize(int type) {#setPaperSize-int-}
```
public void setPaperSize(int type)
```


根据默认打印机的设置设置默认打印纸张大小。

**Remarks**

如果没有纸张大小设置，MS Excel 将使用默认打印机的设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [PaperSizeType](../../com.aspose.cells/papersizetype)。默认纸张大小。 |

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

### setPreferredParsers(ICustomParser[] value) {#setPreferredParsers-com.aspose.cells.ICustomParser---}
```
public void setPreferredParsers(ICustomParser[] value)
```


设置加载文本文件的首选值解析器。

**Remarks**

parsers[0] 是用于文本模板文件第一列的解析器，parsers[1] 是用于第二列的解析器，...等。最后一个（parsers[parsers.length-1]）将用于从 parsers.length-1 开始的所有其他列。如果某个项为 null，则相应列将使用 Aspose.Cells 的默认解析器进行解析。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [ICustomParser\[\]](../../com.aspose.cells/icustomparser) |  |

### setPreservePaddingSpacesInFormula(boolean value) {#setPreservePaddingSpacesInFormula-boolean-}
```
public void setPreservePaddingSpacesInFormula(boolean value)
```


指示在获取和设置公式时是否保留公式标记之间填充的空格和换行。默认值为 false。

**Remarks**

使用此选项从模板文件加载工作簿后，[FormulaSettings.getPreservePaddingSpaces()](../../com.aspose.cells/formulasettings\#getPreservePaddingSpaces--) 将被设置为与此属性相同的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setRegion(int value) {#setRegion-int-}
```
public void setRegion(int value)
```


设置将要加载的工作簿使用的区域设置。

参见 [CountryCode](../../com.aspose.cells/countrycode)。

**Remarks**

区域设置可用于初始化工作簿的一些功能，例如字体、主题等。对于基于文本的文件格式，如 CSV、HTML 等，区域设置还将用于检测数字格式并将文本值解析为单元格的数值或日期时间值。此设置将在后续实例化的工作簿中保留，即工作簿的 [WorkbookSettings.getRegion()](../../com.aspose.cells/workbooksettings\#getRegion--) 将使用与此属性相同的区域。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

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

### setStandardFont(String value) {#setStandardFont-java.lang.String-}
```
public void setStandardFont(String value)
```


设置默认标准字体名称

**Remarks**

注意：此成员现已过时。请改用 DefaultStyleSettings。此属性将在自 2022 年 3 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setStandardFontSize(double value) {#setStandardFontSize-double-}
```
public void setStandardFontSize(double value)
```


设置默认标准字体大小。

**Remarks**

注意：此成员现已过时。请改用 DefaultStyleSettings。此属性将在自 2022 年 3 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setTextQualifier(char value) {#setTextQualifier-char-}
```
public void setTextQualifier(char value)
```


指定单元格值的文本限定符。默认限定符为 '"'。

**Remarks**

设置此属性时，[hasTextQualifier()](../../com.aspose.cells/txtloadoptions\\#hasTextQualifier--) 将自动变为 true。

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


指示是否应将前导单引号视为单元格值的一部分。默认值为 true。如果为 false，前导单引号将从相应单元格的值中移除，并且 [Style.getQuotePrefix()](../../com.aspose.cells/style\\#getQuotePrefix--) 将被设置为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```


设置警告回调。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |

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

