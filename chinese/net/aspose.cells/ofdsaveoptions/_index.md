---
title: "类 OfdSaveOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.OfdSaveOptions 类。表示保存 OFDOpen 固定布局文档文件的选项"
type: docs
url: /zh/net/aspose.cells/ofdsaveoptions/
---
## OfdSaveOptions class

表示保存 OFD（开放固定布局文档）文件的选项。

```csharp
public class OfdSaveOptions : PaginatedSaveOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [OfdSaveOptions](ofdsaveoptions/)() | 创建保存 OFD 文件的选项。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells/paginatedsaveoptions/allcolumnsinonepagepersheet/) { get; set; } | 如果 AllColumnsInOnePagePerSheet 为 true，则一个工作表的所有列内容将在结果中输出到仅一页。pagesetup 的纸张尺寸宽度将被忽略，pagesetup 的其他设置仍然生效。（继承自 [`PaginatedSaveOptions`](../paginatedsaveoptions/)。） |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | 用于临时文件的文件夹，可用作数据缓存。（继承自 [`SaveOptions`](../saveoptions/)。） |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | 是否在用户修改单元格相关对象时检查 Excel 文件的限制。例如，Excel 不允许输入超过 32K 的字符串值。当您输入超过 32K 的值时，它将被截断。（继承自 [`SaveOptions`](../saveoptions/)。） |
| [CheckFontCompatibility](../../aspose.cells/paginatedsaveoptions/checkfontcompatibility/) { get; set; } | 指示是否检查文本中每个字符的字体兼容性。（继承自 [`PaginatedSaveOptions`](../paginatedsaveoptions/)。） |
| [CheckWorkbookDefaultFont](../../aspose.cells/paginatedsaveoptions/checkworkbookdefaultfont/) { get; set; } | 当 Excel 中的字符是 Unicode 且未在单元格样式中设置正确的字体时，它们可能在 pdf、image 中显示为方块。将此设置为 true 以尝试首先使用工作簿的默认字体显示这些字符。（Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).） |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | 在保存文件后使工作簿为空。（Inherited from [`SaveOptions`](../saveoptions/).） |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | 如果为 true 且目录不存在，目录将在保存文件之前自动创建。（Inherited from [`SaveOptions`](../saveoptions/).） |
| [CustomRenderSettings](../../aspose.cells/paginatedsaveoptions/customrendersettings/) { get; set; } | 获取或设置渲染期间的自定义设置。（Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).） |
| [DefaultEditLanguage](../../aspose.cells/paginatedsaveoptions/defaulteditlanguage/) { get; set; } | 获取或设置默认编辑语言。（Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).） |
| [DefaultFont](../../aspose.cells/paginatedsaveoptions/defaultfont/) { get; set; } | 当 Excel 中的字符是 Unicode 且未在单元格样式中设置正确的字体时，它们可能在 pdf、image 中显示为方块。将 DefaultFont 设置为如 MingLiu 或 MS Gothic 以显示这些字符。如果未设置此属性，Aspose.Cells 将使用系统默认字体显示这些 Unicode 字符。（Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).） |
| [DrawObjectEventHandler](../../aspose.cells/paginatedsaveoptions/drawobjecteventhandler/) { get; set; } | 实现此接口以在渲染时获取 DrawObject 和 Bound。（Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).） |
| [EmfRenderSetting](../../aspose.cells/paginatedsaveoptions/emfrendersetting/) { get; set; } | 用于渲染 Emf 元文件的设置。（Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).） |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | 指示在保存为 .xls 文件时是否加密文档属性。默认值为 true。（Inherited from [`SaveOptions`](../saveoptions/).） |
| [GridlineColor](../../aspose.cells/paginatedsaveoptions/gridlinecolor/) { get; set; } | 获取或设置网格线颜色。（Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).） |
| [GridlineType](../../aspose.cells/paginatedsaveoptions/gridlinetype/) { get; set; } | 获取或设置网格线类型。（Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).） |
| [IgnoreError](../../aspose.cells/paginatedsaveoptions/ignoreerror/) { get; set; } | 指示是否需要在渲染时隐藏错误。错误可能出现在形状、图像、图表渲染等方面。（Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).） |
| [IsFontSubstitutionCharGranularity](../../aspose.cells/paginatedsaveoptions/isfontsubstitutionchargranularity/) { get; set; } | 指示是否仅在单元格字体不兼容时替换字符的字体。（Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).） |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | 指示是否在保存文件前合并条件格式和验证的区域。（Inherited from [`SaveOptions`](../saveoptions/).） |
| [OnePagePerSheet](../../aspose.cells/paginatedsaveoptions/onepagepersheet/) { get; set; } | 如果 OnePagePerSheet 为 true，单个工作表的所有内容将仅输出到结果中的一页。pagesetup 的纸张大小将失效，而 pagesetup 的其他设置仍然生效。（Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).） |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells/paginatedsaveoptions/outputblankpagewhennothingtoprint/) { get; set; } | 指示在没有内容可打印时是否输出空白页。（Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).） |
| [PageCount](../../aspose.cells/paginatedsaveoptions/pagecount/) { get; set; } | 获取或设置要保存的页数。（Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).） |
| [PageIndex](../../aspose.cells/paginatedsaveoptions/pageindex/) { get; set; } | 获取或设置要保存的第一页的 0 基索引。（Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).） |
| [PageSavingCallback](../../aspose.cells/paginatedsaveoptions/pagesavingcallback/) { get; set; } | 控制/指示页面保存过程的进度。（Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).） |
| [PrintingPageType](../../aspose.cells/paginatedsaveoptions/printingpagetype/) { get; set; } | 指示哪些页面不会被打印。（Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).） |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | 指示是否缓存图表的最新数据。（Inherited from [`SaveOptions`](../saveoptions/).） |
| [RenderingBehavior](../../aspose.cells/paginatedsaveoptions/renderingbehavior/) { get; set; } | 获取或设置要应用的特定于 Excel 的渲染行为。（Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).） |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | 获取保存的文件格式。（Inherited from [`SaveOptions`](../saveoptions/).） |
| [SheetSet](../../aspose.cells/paginatedsaveoptions/sheetset/) { get; set; } | 获取或设置要渲染的工作表。默认是工作簿中所有可见的工作表：[`Visible`](../../aspose.cells.rendering/sheetset/visible/).（Inherited from [`PaginatedSaveOptions`](../paginatedsaveoptions/).） |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | 指示是否在保存文件前对外部定义的名称进行排序。（Inherited from [`SaveOptions`](../saveoptions/).） |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | 指示是否在保存文件之前对已定义的名称进行排序。（继承自 [`SaveOptions`](../saveoptions/)。） |
| [TextCrossType](../../aspose.cells/paginatedsaveoptions/textcrosstype/) { get; set; } | 获取或设置当文本宽度大于单元格宽度时的显示文本类型。（继承自 [`PaginatedSaveOptions`](../paginatedsaveoptions/)。） |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | 指示是否更新 Smart Art 设置。默认值为 false。（继承自 [`SaveOptions`](../saveoptions/)。） |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | 指示是否在保存文件之前验证合并单元格。（继承自 [`SaveOptions`](../saveoptions/)。） |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | 获取或设置警告回调。（继承自 [`SaveOptions`](../saveoptions/)。） |

### 另请参见

* class [PaginatedSaveOptions](../paginatedsaveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


