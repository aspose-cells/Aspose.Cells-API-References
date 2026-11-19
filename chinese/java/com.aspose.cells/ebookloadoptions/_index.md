---
title: "EbookLoadOptions"
second_title: "Aspose.Cells for Java API 参考"
description: "表示导入电子书文件时的选项。"
type: docs
url: /zh/java/com.aspose.cells/ebookloadoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LoadOptions](../../com.aspose.cells/loadoptions), [com.aspose.cells.AbstractTextLoadOptions](../../com.aspose.cells/abstracttextloadoptions), [com.aspose.cells.HtmlLoadOptions](../../com.aspose.cells/htmlloadoptions)
```
public class EbookLoadOptions extends HtmlLoadOptions
```

表示导入电子书文件时的选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [EbookLoadOptions()](#EbookLoadOptions--) | 创建用于加载电子书文件的选项。 |
| [EbookLoadOptions(int loadFormat)](#EbookLoadOptions-int-) | 创建加载电子书文件的选项。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAttachedFilesDirectory()](#getAttachedFilesDirectory--) | 附件文件将保存到的目录。 |
| [getAutoFilter()](#getAutoFilter--) | 指示在加载文件时是否自动过滤数据。 |
| [getAutoFitColsAndRows()](#getAutoFitColsAndRows--) | 指示是否自动适配列和行。 |
| [getAutoFitterOptions()](#getAutoFitterOptions--) | 获取自动适配选项 |
| [getCheckDataValid()](#getCheckDataValid--) | 检查模板文件中的数据是否有效。 |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | 是否在用户修改单元格相关对象时检查 Excel 文件的限制。 |
| [getClass()](#getClass--) |  |
| [getConvertDateTimeData()](#getConvertDateTimeData--) | 获取一个值，指示文本文件中的字符串是否转换为日期数据。 |
| [getConvertFormulasData()](#getConvertFormulasData--) | 如果为 true，则在字符串值以字符 '=' 开头时将其转换为公式，默认值为 false。 |
| [getConvertNumericData()](#getConvertNumericData--) | 获取一个值，指示文本文件中的字符串是否转换为数值数据。 |
| [getDefaultStyleSettings()](#getDefaultStyleSettings--) | 获取用于初始化工作簿样式的默认样式设置 |
| [getDeleteRedundantSpaces()](#getDeleteRedundantSpaces--) | 指示在使用 `<br>` 标签换行时是否删除多余的空格。 |
| [getDetectLaTeX()](#getDetectLaTeX--) | 指示是否在 HTML 文件中检测 LaTeX 公式。 |
| [getEncoding()](#getEncoding--) | 获取默认编码。 |
| [getFontConfigs()](#getFontConfigs--) | 获取单独的字体配置。 |
| [getHyperlinkLoadMode()](#getHyperlinkLoadMode--) | 指定加载 HTML 时超链接的加载方式。 |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--) | 忽略直接打印文件时未打印的数据 |
| [getIgnoreUselessShapes()](#getIgnoreUselessShapes--) | 指示是否忽略无用的形状。 |
| [getInterruptMonitor()](#getInterruptMonitor--) | 获取中断监视器。 |
| [getKeepPrecision()](#getKeepPrecision--) | 指示当字符串长度为 15 时是否不解析该字符串值。 |
| [getKeepUnparsedData()](#getKeepUnparsedData--) | 是否在从模板文件加载工作簿时将未解析的数据保留在内存中。 |
| [getLanguageCode()](#getLanguageCode--) | 获取基于已保存文件的 CountryCode 的工作簿版本的用户界面语言。 |
| [getLightCellsDataHandler()](#getLightCellsDataHandler--) | 读取模板文件时用于处理单元格数据的数据处理程序。 |
| [getLoadFilter()](#getLoadFilter--) | 用于指示如何加载数据的过滤器。 |
| [getLoadFormat()](#getLoadFormat--) | 获取加载格式。 |
| [getLoadFormulas()](#getLoadFormulas--) | 指示如果原始 HTML 文件包含公式时是否导入公式。 |
| [getLoadStyleStrategy()](#getLoadStyleStrategy--) | 指示在将字符串值转换为数字或日期时间时，对解析值应用样式的策略。 |
| [getLocale()](#getLocale--) | 获取将要加载的工作簿使用的区域设置。 |
| [getMemorySetting()](#getMemorySetting--) | 获取已加载工作簿的内存模式。 |
| [getParagrahLayoutMode()](#getParagrahLayoutMode--) | 指定在加载 HTML 时 HTML <p> 元素的渲染方式。 |
| [getParagraphLayoutMode()](#getParagraphLayoutMode--) | 指定在加载 HTML 时 HTML <p> 元素的渲染方式。 |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | 指示在读取文件时是否解析公式。 |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--) | 指示在加载文件时是否解析数据透视表缓存记录。 |
| [getPassword()](#getPassword--) | 获取工作簿的密码。 |
| [getPreservePaddingSpacesInFormula()](#getPreservePaddingSpacesInFormula--) | 指示在获取和设置公式时是否保留公式标记之间填充的空格和换行符。 |
| [getProgId()](#getProgId--) | 获取创建文件的程序 ID。 |
| [getRegion()](#getRegion--) | 获取将要加载的工作簿使用的区域设置。 |
| [getStandardFont()](#getStandardFont--) | 设置默认标准字体名称 |
| [getStandardFontSize()](#getStandardFontSize--) | 设置默认标准字体大小。 |
| [getStreamProvider()](#getStreamProvider--) | 获取用于导入对象的 StreamProviderImportHtmlFile。 |
| [getSupportDivTag()](#getSupportDivTag--) | 指示当 HTML 文件包含 `<div>` 标记时是否支持其布局。 |
| [getTableLoadOptions()](#getTableLoadOptions--) | 获取 HtmlTableLoadOptionCollection 实例 |
| [getWarningCallback()](#getWarningCallback--) | 获取警告回调。 |
| [hasFormula()](#hasFormula--) | 指示如果文本以 "=" 开头，则是否为公式。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAttachedFilesDirectory(String value)](#setAttachedFilesDirectory-java.lang.String-) | 附件文件将保存到的目录。 |
| [setAutoFilter(boolean value)](#setAutoFilter-boolean-) | 指示在加载文件时是否自动过滤数据。 |
| [setAutoFitColsAndRows(boolean value)](#setAutoFitColsAndRows-boolean-) | 指示是否自动适配列和行。 |
| [setAutoFitterOptions(AutoFitterOptions value)](#setAutoFitterOptions-com.aspose.cells.AutoFitterOptions-) | 设置自动适配选项 |
| [setCheckDataValid(boolean value)](#setCheckDataValid-boolean-) | 检查模板文件中的数据是否有效。 |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | 是否在用户修改单元格相关对象时检查 Excel 文件的限制。 |
| [setConvertDateTimeData(boolean value)](#setConvertDateTimeData-boolean-) | 设置一个值，指示文本文件中的字符串是否转换为日期数据。 |
| [setConvertFormulasData(boolean value)](#setConvertFormulasData-boolean-) | 如果为 true，则在字符串值以字符 '=' 开头时将其转换为公式，默认值为 false。 |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | 设置一个值，指示文本文件中的字符串是否转换为数值数据。 |
| [setDeleteRedundantSpaces(boolean value)](#setDeleteRedundantSpaces-boolean-) | 指示在使用 `<br>` 标签换行时是否删除多余的空格。 |
| [setDetectLaTeX(boolean value)](#setDetectLaTeX-boolean-) | 指示是否在 HTML 文件中检测 LaTeX 公式。 |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | 设置默认编码。 |
| [setFontConfigs(IndividualFontConfigs value)](#setFontConfigs-com.aspose.cells.IndividualFontConfigs-) | 设置单个字体配置。 |
| [setHasFormula(boolean value)](#setHasFormula-boolean-) | 指示如果文本以 "=" 开头，则是否为公式。 |
| [setHyperlinkLoadMode(int value)](#setHyperlinkLoadMode-int-) | 指定加载 HTML 时超链接的加载方式。 |
| [setIgnoreNotPrinted(boolean value)](#setIgnoreNotPrinted-boolean-) | 忽略直接打印文件时未打印的数据 |
| [setIgnoreUselessShapes(boolean value)](#setIgnoreUselessShapes-boolean-) | 指示是否忽略无用的形状。 |
| [setInterruptMonitor(AbstractInterruptMonitor value)](#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-) | 设置中断监视器。 |
| [setKeepPrecision(boolean value)](#setKeepPrecision-boolean-) | 指示当字符串长度为 15 时是否不解析该字符串值。 |
| [setKeepUnparsedData(boolean value)](#setKeepUnparsedData-boolean-) | 是否在从模板文件加载工作簿时将未解析的数据保留在内存中。 |
| [setLanguageCode(int value)](#setLanguageCode-int-) | 根据保存文件的 CountryCode 设置工作簿版本的用户界面语言。 |
| [setLightCellsDataHandler(LightCellsDataHandler value)](#setLightCellsDataHandler-com.aspose.cells.LightCellsDataHandler-) | 读取模板文件时用于处理单元格数据的数据处理程序。 |
| [setLoadFilter(LoadFilter value)](#setLoadFilter-com.aspose.cells.LoadFilter-) | 用于指示如何加载数据的过滤器。 |
| [setLoadFormulas(boolean value)](#setLoadFormulas-boolean-) | 指示如果原始 HTML 文件包含公式时是否导入公式。 |
| [setLoadStyleStrategy(int value)](#setLoadStyleStrategy-int-) | 指示在将字符串值转换为数字或日期时间时，对解析值应用样式的策略。 |
| [setLocale(Locale value)](#setLocale-java.util.Locale-) | 设置将要加载的工作簿使用的区域设置。 |
| [setMemorySetting(int value)](#setMemorySetting-int-) | 设置已加载工作簿的内存模式。 |
| [setPaperSize(int type)](#setPaperSize-int-) | 根据默认打印机的设置设置默认打印纸张大小。 |
| [setParagrahLayoutMode(int value)](#setParagrahLayoutMode-int-) | 指定在加载 HTML 时 HTML <p> 元素的渲染方式。 |
| [setParagraphLayoutMode(int value)](#setParagraphLayoutMode-int-) | 指定在加载 HTML 时 HTML <p> 元素的渲染方式。 |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | 指示在读取文件时是否解析公式。 |
| [setParsingPivotCachedRecords(boolean value)](#setParsingPivotCachedRecords-boolean-) | 指示在加载文件时是否解析数据透视表缓存记录。 |
| [setPassword(String value)](#setPassword-java.lang.String-) | 设置工作簿的密码。 |
| [setPreservePaddingSpacesInFormula(boolean value)](#setPreservePaddingSpacesInFormula-boolean-) | 指示在获取和设置公式时是否保留公式标记之间填充的空格和换行符。 |
| [setRegion(int value)](#setRegion-int-) | 设置将要加载的工作簿使用的区域设置。 |
| [setStandardFont(String value)](#setStandardFont-java.lang.String-) | 设置默认标准字体名称 |
| [setStandardFontSize(double value)](#setStandardFontSize-double-) | 设置默认标准字体大小。 |
| [setStreamProvider(IStreamProvider value)](#setStreamProvider-com.aspose.cells.IStreamProvider-) | 设置用于导入对象的 StreamProviderImportHtmlFile。 |
| [setSupportDivTag(boolean value)](#setSupportDivTag-boolean-) | 指示当 HTML 文件包含 `<div>` 标记时是否支持其布局。 |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | 设置警告回调。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### EbookLoadOptions() {#EbookLoadOptions--}
```
public EbookLoadOptions()
```


创建用于加载电子书文件的选项。

### EbookLoadOptions(int loadFormat) {#EbookLoadOptions-int-}
```
public EbookLoadOptions(int loadFormat)
```


创建加载电子书文件的选项。

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
### getAttachedFilesDirectory() {#getAttachedFilesDirectory--}
```
public String getAttachedFilesDirectory()
```


附件文件将保存到的目录。

**Remarks**

注意：此成员现已过时。请改用 HtmlLoadOptions.StreamProvider 属性。该属性将在自 2014 年 12 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
java.lang.String
### getAutoFilter() {#getAutoFilter--}
```
public boolean getAutoFilter()
```


指示在加载文件时是否自动过滤数据。

**Remarks**

有时即使已设置自动筛选，文件中相应的行仍未隐藏。现在仅适用于 SpreadSheetML 文件。

**Returns:**
boolean
### getAutoFitColsAndRows() {#getAutoFitColsAndRows--}
```
public boolean getAutoFitColsAndRows()
```


指示是否自动调整列和行的大小。默认值为 false。

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
### getConvertFormulasData() {#getConvertFormulasData--}
```
public boolean getConvertFormulasData()
```


如果为 true，则在字符串值以字符 '=' 开头时将其转换为公式，默认值为 false。

**Remarks**

注意：此属性现已过时。请改用 HtmlLoadOptions.HasFormula 属性。该属性将在自 2023 年 3 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

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
### getDeleteRedundantSpaces() {#getDeleteRedundantSpaces--}
```
public boolean getDeleteRedundantSpaces()
```


指示在使用 `<br>` 标记换行时是否删除多余的空格。默认值为 false。

**Returns:**
boolean
### getDetectLaTeX() {#getDetectLaTeX--}
```
public boolean getDetectLaTeX()
```


指示是否在 HTML 文件中检测 LaTeX 公式。默认值为 false。

**Returns:**
boolean
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


获取默认编码。仅适用于 csv 文件。

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getFontConfigs() {#getFontConfigs--}
```
public IndividualFontConfigs getFontConfigs()
```


获取单个字体配置。仅适用于使用此 [LoadOptions](../../com.aspose.cells/loadoptions) 加载的 [Workbook](../../com.aspose.cells/workbook)。

**Returns:**
[IndividualFontConfigs](../../com.aspose.cells/individualfontconfigs)
### getHyperlinkLoadMode() {#getHyperlinkLoadMode--}
```
public int getHyperlinkLoadMode()
```


指定加载 HTML 时超链接的加载方式。

参见 [HyperlinkLoadMode](../../com.aspose.cells/hyperlinkloadmode)。

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
### getLoadFormulas() {#getLoadFormulas--}
```
public boolean getLoadFormulas()
```


指示如果原始 HTML 文件包含公式时是否导入公式。

**Returns:**
boolean
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
### getParagrahLayoutMode() {#getParagrahLayoutMode--}
```
public int getParagrahLayoutMode()
```


指定在加载 HTML 时如何呈现 HTML <p> 元素。默认值为 [HtmlParagraphLayoutMode.NORMAL](../../com.aspose.cells/htmlparagraphlayoutmode\#NORMAL)。

参见 [HtmlParagraphLayoutMode](../../com.aspose.cells/htmlparagraphlayoutmode)。

**Remarks**

注意：此属性现已过时。请改用 HtmlLoadOptions.ParagraphLayoutMode 属性。该方法将在自 2026 年 7 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
int
### getParagraphLayoutMode() {#getParagraphLayoutMode--}
```
public int getParagraphLayoutMode()
```


指定在加载 HTML 时如何呈现 HTML <p> 元素。默认值为 [HtmlParagraphLayoutMode.NORMAL](../../com.aspose.cells/htmlparagraphlayoutmode\#NORMAL)。

参见 [HtmlParagraphLayoutMode](../../com.aspose.cells/htmlparagraphlayoutmode)。

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
### getPreservePaddingSpacesInFormula() {#getPreservePaddingSpacesInFormula--}
```
public boolean getPreservePaddingSpacesInFormula()
```


指示在获取和设置公式时是否保留公式标记之间填充的空格和换行。默认值为 false。

**Remarks**

使用此选项从模板文件加载工作簿后，[FormulaSettings.getPreservePaddingSpaces()](../../com.aspose.cells/formulasettings\#getPreservePaddingSpaces--) 将被设置为与此属性相同的值。

**Returns:**
boolean
### getProgId() {#getProgId--}
```
public String getProgId()
```


获取创建文件的程序 ID。仅适用于 MHT 文件。

**Returns:**
java.lang.String
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
### getStreamProvider() {#getStreamProvider--}
```
public IStreamProvider getStreamProvider()
```


获取用于导入对象的 StreamProviderImportHtmlFile。

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getSupportDivTag() {#getSupportDivTag--}
```
public boolean getSupportDivTag()
```


指示当 HTML 文件包含 `<div>` 标记时是否支持其布局。默认值为 false。

**Returns:**
boolean
### getTableLoadOptions() {#getTableLoadOptions--}
```
public HtmlTableLoadOptionCollection getTableLoadOptions()
```


获取 HtmlTableLoadOptionCollection 实例

**Returns:**
[HtmlTableLoadOptionCollection](../../com.aspose.cells/htmltableloadoptioncollection)
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




### setAttachedFilesDirectory(String value) {#setAttachedFilesDirectory-java.lang.String-}
```
public void setAttachedFilesDirectory(String value)
```


附件文件将保存到的目录。

**Remarks**

注意：此成员现已过时。请改用 HtmlLoadOptions.StreamProvider 属性。该属性将在自 2014 年 12 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

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

### setAutoFitColsAndRows(boolean value) {#setAutoFitColsAndRows-boolean-}
```
public void setAutoFitColsAndRows(boolean value)
```


指示是否自动调整列和行的大小。默认值为 false。

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

### setConvertFormulasData(boolean value) {#setConvertFormulasData-boolean-}
```
public void setConvertFormulasData(boolean value)
```


如果为 true，则在字符串值以字符 '=' 开头时将其转换为公式，默认值为 false。

**Remarks**

注意：此属性现已过时。请改用 HtmlLoadOptions.HasFormula 属性。该属性将在自 2023 年 3 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

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

### setDeleteRedundantSpaces(boolean value) {#setDeleteRedundantSpaces-boolean-}
```
public void setDeleteRedundantSpaces(boolean value)
```


指示在使用 `<br>` 标记换行时是否删除多余的空格。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setDetectLaTeX(boolean value) {#setDetectLaTeX-boolean-}
```
public void setDetectLaTeX(boolean value)
```


指示是否在 HTML 文件中检测 LaTeX 公式。默认值为 false。

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

### setHyperlinkLoadMode(int value) {#setHyperlinkLoadMode-int-}
```
public void setHyperlinkLoadMode(int value)
```


指定加载 HTML 时超链接的加载方式。

参见 [HyperlinkLoadMode](../../com.aspose.cells/hyperlinkloadmode)。

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

### setLoadFormulas(boolean value) {#setLoadFormulas-boolean-}
```
public void setLoadFormulas(boolean value)
```


指示如果原始 HTML 文件包含公式时是否导入公式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

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

### setParagrahLayoutMode(int value) {#setParagrahLayoutMode-int-}
```
public void setParagrahLayoutMode(int value)
```


指定在加载 HTML 时如何呈现 HTML <p> 元素。默认值为 [HtmlParagraphLayoutMode.NORMAL](../../com.aspose.cells/htmlparagraphlayoutmode\#NORMAL)。

参见 [HtmlParagraphLayoutMode](../../com.aspose.cells/htmlparagraphlayoutmode)。

**Remarks**

注意：此属性现已过时。请改用 HtmlLoadOptions.ParagraphLayoutMode 属性。该方法将在自 2026 年 7 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setParagraphLayoutMode(int value) {#setParagraphLayoutMode-int-}
```
public void setParagraphLayoutMode(int value)
```


指定在加载 HTML 时如何呈现 HTML <p> 元素。默认值为 [HtmlParagraphLayoutMode.NORMAL](../../com.aspose.cells/htmlparagraphlayoutmode\#NORMAL)。

参见 [HtmlParagraphLayoutMode](../../com.aspose.cells/htmlparagraphlayoutmode)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

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

### setStreamProvider(IStreamProvider value) {#setStreamProvider-com.aspose.cells.IStreamProvider-}
```
public void setStreamProvider(IStreamProvider value)
```


设置用于导入对象的 StreamProviderImportHtmlFile。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setSupportDivTag(boolean value) {#setSupportDivTag-boolean-}
```
public void setSupportDivTag(boolean value)
```


指示当 HTML 文件包含 `<div>` 标记时是否支持其布局。默认值为 false。

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

