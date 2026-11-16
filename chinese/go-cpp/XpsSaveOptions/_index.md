---
title: "XpsSaveOptions 类"
linktitle: "XpsSaveOptions"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "XpsSaveOptions 类。封装了在 Go 中表示 xpssaveoptions 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/xpssaveoptions/
---

## XpsSaveOptions class

表示将文件保存为 Xps 时的附加选项。

```go

type XpsSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewXpsSaveOptions](./newxpssaveoptions/) | 创建用于保存 xps 文件的选项。 |
| [NewXpsSaveOptions_PaginatedSaveOptions](./newxpssaveoptions_paginatedsaveoptions/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetDefaultFont](./getdefaultfont/) | 当 Excel 中的字符是 Unicode 且单元格样式未设置正确字体时，它们可能在 pdf、图像中显示为方块。请将 DefaultFont 设置为如 MingLiu 或 MS Gothic 等字体以显示这些字符。如果未设置此属性，Aspose.Cells 将使用系统默认字体来显示这些 Unicode 字符。 |
| [SetDefaultFont](./setdefaultfont/) | 当 Excel 中的字符是 Unicode 且单元格样式未设置正确字体时，它们可能在 pdf、图像中显示为方块。请将 DefaultFont 设置为如 MingLiu 或 MS Gothic 等字体以显示这些字符。如果未设置此属性，Aspose.Cells 将使用系统默认字体来显示这些 Unicode 字符。 |
| [GetCheckWorkbookDefaultFont](./getcheckworkbookdefaultfont/) | 当 Excel 中的字符是 Unicode 且单元格样式未设置正确字体时，它们可能在 pdf、图像中显示为方块。将此设置为 true，以尝试首先使用工作簿的默认字体来显示这些字符。 |
| [SetCheckWorkbookDefaultFont](./setcheckworkbookdefaultfont/) | 当 Excel 中的字符是 Unicode 且单元格样式未设置正确字体时，它们可能在 pdf、图像中显示为方块。将此设置为 true，以尝试首先使用工作簿的默认字体来显示这些字符。 |
| [SetCheckFontCompatibility](./setcheckfontcompatibility/) | 指示是否检查文本中每个字符的字体兼容性。 |
| [GetCheckFontCompatibility](./getcheckfontcompatibility/) | 指示是否检查文本中每个字符的字体兼容性。 |
| [SetIsFontSubstitutionCharGranularity](./setisfontsubstitutionchargranularity/) | 指示是否仅在单元格字体与字符不兼容时替换该字符的字体。 |
| [IsFontSubstitutionCharGranularity](./isfontsubstitutionchargranularity/) | 指示是否仅在单元格字体与字符不兼容时替换该字符的字体。 |
| [GetOnePagePerSheet](./getonepagepersheet/) | 如果 OnePagePerSheet 为 true，则一个工作表的所有内容将输出到结果中的唯一一页。pagesetup 的纸张大小将失效，但 pagesetup 的其他设置仍会生效。 |
| [SetOnePagePerSheet](./setonepagepersheet/) | 如果 OnePagePerSheet 为 true，则一个工作表的所有内容将输出到结果中的唯一一页。pagesetup 的纸张大小将失效，但 pagesetup 的其他设置仍会生效。 |
| [GetAllColumnsInOnePagePerSheet](./getallcolumnsinonepagepersheet/) | 如果 AllColumnsInOnePagePerSheet 为 true，则一个工作表的所有列内容将输出到结果中的唯一一页。pagesetup 的纸张宽度将被忽略，但 pagesetup 的其他设置仍会生效。 |
| [SetAllColumnsInOnePagePerSheet](./setallcolumnsinonepagepersheet/) | 如果 AllColumnsInOnePagePerSheet 为 true，则一个工作表的所有列内容将输出到结果中的唯一一页。pagesetup 的纸张宽度将被忽略，但 pagesetup 的其他设置仍会生效。 |
| [GetIgnoreError](./getignoreerror/) | 指示在渲染时是否需要隐藏错误。错误可能出现在形状、图像、图表渲染等方面。 |
| [SetIgnoreError](./setignoreerror/) | 指示在渲染时是否需要隐藏错误。错误可能出现在形状、图像、图表渲染等方面。 |
| [GetOutputBlankPageWhenNothingToPrint](./getoutputblankpagewhennothingtoprint/) | 指示在没有内容可打印时是否输出空白页。 |
| [SetOutputBlankPageWhenNothingToPrint](./setoutputblankpagewhennothingtoprint/) | 指示在没有内容可打印时是否输出空白页。 |
| [SetPageIndex](./setpageindex/) | 获取或设置要保存的第一页的基于 0 的索引。 |
| [GetPageIndex](./getpageindex/) | 获取或设置要保存的第一页的基于 0 的索引。 |
| [SetPageCount](./setpagecount/) | 获取或设置要保存的页数。 |
| [GetPageCount](./getpagecount/) | 获取或设置要保存的页数。 |
| [GetPrintingPageType](./getprintingpagetype/) | 指示哪些页面将不被打印。 |
| [SetPrintingPageType](./setprintingpagetype/) | 指示哪些页面将不被打印。 |
| [GetGridlineType](./getgridlinetype/) | 获取或设置网格线类型。 |
| [SetGridlineType](./setgridlinetype/) | 获取或设置网格线类型。 |
| [GetGridlineColor](./getgridlinecolor/) | 获取或设置网格线颜色。 |
| [SetGridlineColor](./setgridlinecolor/) | 获取或设置网格线颜色。 |
| [GetTextCrossType](./gettextcrosstype/) | 获取或设置当文本宽度大于单元格宽度时的显示文本类型。 |
| [SetTextCrossType](./settextcrosstype/) | 获取或设置当文本宽度大于单元格宽度时的显示文本类型。 |
| [GetDefaultEditLanguage](./getdefaulteditlanguage/) | 获取或设置默认编辑语言。 |
| [SetDefaultEditLanguage](./setdefaulteditlanguage/) | 获取或设置默认编辑语言。 |
| [GetSheetSet](./getsheetset/) | 获取或设置要渲染的工作表。默认是工作簿中所有可见的工作表：Aspose.Cells.Rendering.SheetSet.Visible。 |
| [SetSheetSet](./setsheetset/) | 获取或设置要渲染的工作表。默认是工作簿中所有可见的工作表：Aspose.Cells.Rendering.SheetSet.Visible。 |
| [GetDrawObjectEventHandler](./getdrawobjecteventhandler/) | 实现此接口以在渲染时获取 DrawObject 和 Bound。 |
| [SetDrawObjectEventHandler](./setdrawobjecteventhandler/) | 实现此接口以在渲染时获取 DrawObject 和 Bound。 |
| [GetEmfRenderSetting](./getemfrendersetting/) | Emf 元文件渲染设置。 |
| [SetEmfRenderSetting](./setemfrendersetting/) | Emf 元文件渲染设置。 |
| [GetCustomRenderSettings](./getcustomrendersettings/) | 获取或设置渲染期间的自定义设置。 |
| [SetCustomRenderSettings](./setcustomrendersettings/) | 获取或设置渲染期间的自定义设置。 |
| [GetRenderingBehavior](./getrenderingbehavior/) | 获取或设置要应用的特定于 Excel 的渲染行为。 |
| [SetRenderingBehavior](./setrenderingbehavior/) | 获取或设置要应用的特定于 Excel 的渲染行为。 |
| [GetSaveFormat](./getsaveformat/) | 获取保存文件的格式。 |
| [GetClearData](./getcleardata/) | 在保存文件后使工作簿为空。 |
| [SetClearData](./setcleardata/) | 在保存文件后使工作簿为空。 |
| [GetCachedFileFolder](./getcachedfilefolder/) | 用于临时文件的文件夹，可用作数据缓存。 |
| [SetCachedFileFolder](./setcachedfilefolder/) | 用于临时文件的文件夹，可用作数据缓存。 |
| [GetValidateMergedAreas](./getvalidatemergedareas/) | 指示是否在保存文件前验证合并单元格。 |
| [SetValidateMergedAreas](./setvalidatemergedareas/) | 指示是否在保存文件前验证合并单元格。 |
| [GetMergeAreas](./getmergeareas/) | 指示是否在保存文件前合并条件格式和验证的区域。 |
| [SetMergeAreas](./setmergeareas/) | 指示是否在保存文件前合并条件格式和验证的区域。 |
| [GetCreateDirectory](./getcreatedirectory/) | 如果为 true 且目录不存在，目录将在保存文件前自动创建。 |
| [SetCreateDirectory](./setcreatedirectory/) | 如果为 true 且目录不存在，目录将在保存文件前自动创建。 |
| [GetSortNames](./getsortnames/) | 指示是否在保存文件前对已定义名称进行排序。 |
| [SetSortNames](./setsortnames/) | 指示是否在保存文件前对已定义名称进行排序。 |
| [GetSortExternalNames](./getsortexternalnames/) | 指示是否在保存文件前对外部已定义名称进行排序。 |
| [SetSortExternalNames](./setsortexternalnames/) | 指示是否在保存文件前对外部已定义名称进行排序。 |
| [GetRefreshChartCache](./getrefreshchartcache/) | 指示是否缓存图表的最新数据。 |
| [SetRefreshChartCache](./setrefreshchartcache/) | 指示是否缓存图表的最新数据。 |
| [GetCheckExcelRestriction](./getcheckexcelrestriction/) | 是否在用户修改与单元格相关的对象时检查 Excel 文件的限制。例如，Excel 不允许输入超过 32K 的字符串值。当输入的值超过 32K 时，将被截断。 |
| [SetCheckExcelRestriction](./setcheckexcelrestriction/) | 是否在用户修改与单元格相关的对象时检查 Excel 文件的限制。例如，Excel 不允许输入超过 32K 的字符串值。当输入的值超过 32K 时，将被截断。 |
| [GetUpdateSmartArt](./getupdatesmartart/) | 指示是否更新 Smart Art 设置。默认值为 false。 |
| [SetUpdateSmartArt](./setupdatesmartart/) | 指示是否更新 Smart Art 设置。默认值为 false。 |
| [GetEncryptDocumentProperties](./getencryptdocumentproperties/) | 指示在保存为 .xls 文件时是否加密文档属性。默认值为 true。 |
| [SetEncryptDocumentProperties](./setencryptdocumentproperties/) | 指示在保存为 .xls 文件时是否加密文档属性。默认值为 true。 |
