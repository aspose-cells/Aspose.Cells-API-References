---
title: "HtmlLoadOptions 类"
linktitle: "HtmlLoadOptions"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "HtmlLoadOptions 类。封装在 Go 中表示 htmlloadoptions 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/htmlloadoptions/
---

## HtmlLoadOptions class

表示导入 HTML 文件时的选项。

```go

type HtmlLoadOptions struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewHtmlLoadOptions](./newhtmlloadoptions/) | 创建加载文件的选项。 |
| [NewHtmlLoadOptions_LoadFormat](./newhtmlloadoptions_loadformat/) | 创建加载文件的选项。 |
| [NewHtmlLoadOptions_AbstractTextLoadOptions](./newhtmlloadoptions_abstracttextloadoptions/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetLoadFormulas](./getloadformulas/) | 指示是否在原始 HTML 文件包含公式时导入公式 |
| [SetLoadFormulas](./setloadformulas/) | 指示是否在原始 HTML 文件包含公式时导入公式 |
| [GetSupportDivTag](./getsupportdivtag/) | 指示在 HTML 文件包含 <c>&lt;div&gt;</c> 标签时是否支持其布局。默认值为 false。 |
| [SetSupportDivTag](./setsupportdivtag/) | 指示在 HTML 文件包含 <c>&lt;div&gt;</c> 标签时是否支持其布局。默认值为 false。 |
| [GetDeleteRedundantSpaces](./getdeleteredundantspaces/) | 指示在使用 <c>&lt;br&gt;</c> 标签换行时是否删除多余的空格。默认值为 false。 |
| [SetDeleteRedundantSpaces](./setdeleteredundantspaces/) | 指示在使用 <c>&lt;br&gt;</c> 标签换行时是否删除多余的空格。默认值为 false。 |
| [GetAutoFitColsAndRows](./getautofitcolsandrows/) | 指示是否自动适应列和行。默认值为 false。 |
| [SetAutoFitColsAndRows](./setautofitcolsandrows/) | 指示是否自动适应列和行。默认值为 false。 |
| [GetHasFormula](./gethasformula/) | 指示当文本以 "=" 开头时是否为公式。 |
| [SetHasFormula](./sethasformula/) | 指示当文本以 "=" 开头时是否为公式。 |
| [GetProgId](./getprogid/) | 获取创建文件的程序 ID。仅适用于 MHT 文件。 |
| [GetTableLoadOptions](./gettableloadoptions/) | 获取 HtmlTableLoadOptionCollection 实例 |
| [GetDetectLaTeX](./getdetectlatex/) | 指示是否在 HTML 文件中检测 LaTeX 公式。默认值为 false。 |
| [SetDetectLaTeX](./setdetectlatex/) | 指示是否在 HTML 文件中检测 LaTeX 公式。默认值为 false。 |
| [GetParagraphLayoutMode](./getparagraphlayoutmode/) | 指定在加载 HTML 时 HTML &lt;p&gt; 元素的渲染方式。默认值为 HtmlParagraphLayoutMode.Normal。 |
| [SetParagraphLayoutMode](./setparagraphlayoutmode/) | 指定在加载 HTML 时 HTML &lt;p&gt; 元素的渲染方式。默认值为 HtmlParagraphLayoutMode.Normal。 |
| [GetHyperlinkLoadMode](./gethyperlinkloadmode/) | 指定在加载 HTML 时超链接的加载方式。 |
| [SetHyperlinkLoadMode](./sethyperlinkloadmode/) | 指定在加载 HTML 时超链接的加载方式。 |
| [GetEncoding](./getencoding/) | 获取和设置默认编码。仅适用于 csv 文件。 |
| [SetEncoding](./setencoding/) | 获取和设置默认编码。仅适用于 csv 文件。 |
| [GetLoadStyleStrategy](./getloadstylestrategy/) | 指示在将字符串值转换为数字或日期时间时，对解析值应用样式的策略。 |
| [SetLoadStyleStrategy](./setloadstylestrategy/) | 指示在将字符串值转换为数字或日期时间时，对解析值应用样式的策略。 |
| [GetConvertNumericData](./getconvertnumericdata/) | 获取或设置一个值，指示文本文件中的字符串是否转换为数值数据。默认值为 true。 |
| [SetConvertNumericData](./setconvertnumericdata/) | 获取或设置一个值，指示文本文件中的字符串是否转换为数值数据。默认值为 true。 |
| [GetConvertDateTimeData](./getconvertdatetimedata/) | 获取或设置一个值，指示文本文件中的字符串是否转换为日期数据。默认值为 true。 |
| [SetConvertDateTimeData](./setconvertdatetimedata/) | 获取或设置一个值，指示文本文件中的字符串是否转换为日期数据。默认值为 true。 |
| [GetKeepPrecision](./getkeepprecision/) | 指示当字符串长度为 15 时是否不进行解析。 |
| [SetKeepPrecision](./setkeepprecision/) | 指示当字符串长度为 15 时是否不进行解析。 |
| [GetLoadFormat](./getloadformat/) | 获取加载格式。 |
| [GetPassword](./getpassword/) | 获取并设置工作簿的密码。 |
| [SetPassword](./setpassword/) | 获取并设置工作簿的密码。 |
| [GetParsingFormulaOnOpen](./getparsingformulaonopen/) | 指示在读取文件时是否解析公式。 |
| [SetParsingFormulaOnOpen](./setparsingformulaonopen/) | 指示在读取文件时是否解析公式。 |
| [GetParsingPivotCachedRecords](./getparsingpivotcachedrecords/) | 指示在加载文件时是否解析数据透视表缓存记录。默认值为 false。 |
| [SetParsingPivotCachedRecords](./setparsingpivotcachedrecords/) | 指示在加载文件时是否解析数据透视表缓存记录。默认值为 false。 |
| [SetPaperSize](./setpapersize/) | 设置默认打印纸张大小，来源于默认打印机的设置。 |
| [GetLanguageCode](./getlanguagecode/) | 获取或设置基于已保存文件的 CountryCode 的工作簿版本的用户界面语言。 |
| [SetLanguageCode](./setlanguagecode/) | 获取或设置基于已保存文件的 CountryCode 的工作簿版本的用户界面语言。 |
| [GetRegion](./getregion/) | 获取或设置将要加载的工作簿使用的区域设置。 |
| [SetRegion](./setregion/) | 获取或设置将要加载的工作簿使用的区域设置。 |
| [GetDefaultStyleSettings](./getdefaultstylesettings/) | 获取用于初始化工作簿样式的默认样式设置。 |
| [GetInterruptMonitor](./getinterruptmonitor/) | 获取并设置中断监视器。 |
| [SetInterruptMonitor](./setinterruptmonitor/) | 获取并设置中断监视器。 |
| [GetIgnoreNotPrinted](./getignorenotprinted/) | 如果直接打印文件，忽略未打印的数据。 |
| [SetIgnoreNotPrinted](./setignorenotprinted/) | 如果直接打印文件，忽略未打印的数据。 |
| [GetCheckDataValid](./getcheckdatavalid/) | 检查模板文件中的数据是否有效。 |
| [SetCheckDataValid](./setcheckdatavalid/) | 检查模板文件中的数据是否有效。 |
| [GetCheckExcelRestriction](./getcheckexcelrestriction/) | 是否在用户修改单元格相关对象时检查 Excel 文件的限制。例如，Excel 不允许输入超过 32K 的字符串值。当您通过 Cell.PutValue(string) 输入超过 32K 的值时，如果此属性为 true，您将收到异常；如果此属性为 false，我们将接受您输入的字符串值作为单元格的值，以便随后您可以将完整的字符串值输出为其他文件格式，如 CSV。然而，如果您设置了对 Excel 文件格式无效的此类值，之后不应将工作簿保存为 Excel 文件格式。否则生成的 Excel 文件可能会出现意外错误。 |
| [SetCheckExcelRestriction](./setcheckexcelrestriction/) | 是否在用户修改单元格相关对象时检查 Excel 文件的限制。例如，Excel 不允许输入超过 32K 的字符串值。当您通过 Cell.PutValue(string) 输入超过 32K 的值时，如果此属性为 true，您将收到异常；如果此属性为 false，我们将接受您输入的字符串值作为单元格的值，以便随后您可以将完整的字符串值输出为其他文件格式，如 CSV。然而，如果您设置了对 Excel 文件格式无效的此类值，之后不应将工作簿保存为 Excel 文件格式。否则生成的 Excel 文件可能会出现意外错误。 |
| [GetKeepUnparsedData](./getkeepunparseddata/) | 是否在从模板文件加载工作簿时在内存中保留未解析的数据。默认值为 true。 |
| [SetKeepUnparsedData](./setkeepunparseddata/) | 是否在从模板文件加载工作簿时在内存中保留未解析的数据。默认值为 true。 |
| [GetLoadFilter](./getloadfilter/) | 用于指示如何加载数据的过滤器。 |
| [SetLoadFilter](./setloadfilter/) | 用于指示如何加载数据的过滤器。 |
| [GetMemorySetting](./getmemorysetting/) | 获取或设置已加载工作簿的内存模式。 |
| [SetMemorySetting](./setmemorysetting/) | 获取或设置已加载工作簿的内存模式。 |
| [GetAutoFitterOptions](./getautofitteroptions/) | 获取并设置自动适配选项。 |
| [SetAutoFitterOptions](./setautofitteroptions/) | 获取并设置自动适配选项。 |
| [GetAutoFilter](./getautofilter/) | 指示在加载文件时是否自动过滤数据。 |
| [SetAutoFilter](./setautofilter/) | 指示在加载文件时是否自动过滤数据。 |
| [GetFontConfigs](./getfontconfigs/) | 获取并设置各个字体配置。仅适用于使用此 LoadOptions 加载的工作簿。 |
| [SetFontConfigs](./setfontconfigs/) | 获取并设置各个字体配置。仅适用于使用此 LoadOptions 加载的工作簿。 |
| [GetIgnoreUselessShapes](./getignoreuselessshapes/) | 指示是否忽略无用的形状。 |
| [SetIgnoreUselessShapes](./setignoreuselessshapes/) | 指示是否忽略无用的形状。 |
| [GetPreservePaddingSpacesInFormula](./getpreservepaddingspacesinformula/) | 指示在获取和设置公式时是否保留公式标记之间填充的空格和换行符。默认值为 false。 |
| [SetPreservePaddingSpacesInFormula](./setpreservepaddingspacesinformula/) | 指示在获取和设置公式时是否保留公式标记之间填充的空格和换行符。默认值为 false。 |
