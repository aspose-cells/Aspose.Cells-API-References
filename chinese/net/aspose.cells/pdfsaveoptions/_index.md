---
title: PdfSaveOptions
second_title: Aspose.Cells for .NET API 参考
description: 代表保存pdf文件的选项
type: docs
weight: 4500
url: /zh/net/aspose.cells/pdfsaveoptions/
---
## PdfSaveOptions class

代表保存pdf文件的选项。

```csharp
public class PdfSaveOptions : SaveOptions
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions#constructor)() | 创建保存 pdf 文件的选项。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells/pdfsaveoptions/allcolumnsinonepagepersheet) { get; set; } | 如果 AllColumnsInOnePagePerSheet 为 true ，则一张表的所有列内容将只输出到结果中的一页。 pagesetup 的纸张大小宽度将被忽略，pagesetup 的其他设置仍然有效。 |
| [Bookmark](../../aspose.cells/pdfsaveoptions/bookmark) { get; set; } | 获取和设置[`PdfBookmarkEntry`](../../aspose.cells.rendering/pdfbookmarkentry) 对象。 |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder) { get; set; } | 缓存的文件夹是用来存放一些大数据的。 |
| [CalculateFormula](../../aspose.cells/pdfsaveoptions/calculateformula) { get; set; } | 表示是否在保存pdf文件之前计算公式。 |
| [CheckFontCompatibility](../../aspose.cells/pdfsaveoptions/checkfontcompatibility) { get; set; } | 表示是否检查文本中每个字符的字体兼容性。 |
| [CheckWorkbookDefaultFont](../../aspose.cells/pdfsaveoptions/checkworkbookdefaultfont) { get; set; } | 当 Excel 中的字符为 Unicode 且未在单元格样式中设置正确的字体时， 它们可能在 pdf、图像中显示为块。 将此设置为 true 以尝试使用工作簿的默认字体首先显示这些字符。 |
| [ClearData](../../aspose.cells/saveoptions/cleardata) { get; set; } | 保存文件后使工作簿为空。 |
| [Compliance](../../aspose.cells/pdfsaveoptions/compliance) { get; set; } | 工作簿将根据此属性中的 PdfCompliance 转换为 pdf。 |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory) { get; set; } | 如果为true且目录不存在，则在保存文件之前会自动创建目录。 |
| [CreatedTime](../../aspose.cells/pdfsaveoptions/createdtime) { get; set; } | 获取和设置生成pdf文档的时间。 |
| [CustomPropertiesExport](../../aspose.cells/pdfsaveoptions/custompropertiesexport) { get; set; } | 获取或设置一个值，确定[`CustomDocumentPropertyCollection`](../../aspose.cells.properties/customdocumentpropertycollection)导出到 PDF 文件的方式。默认值为无。 |
| [DefaultEditLanguage](../../aspose.cells/pdfsaveoptions/defaulteditlanguage) { get; set; } | 获取或设置默认编辑语言。 |
| [DefaultFont](../../aspose.cells/pdfsaveoptions/defaultfont) { get; set; } | 当 Excel 中的字符为 Unicode 且未在单元格样式中设置正确的字体时， 它们可能在 pdf、图像中显示为块。 设置默认字体如 MingLiu 或 MS Gothic 以显示这些字符。 如果未设置此属性，Aspose.Cells 将使用系统默认字体显示这些 unicode 字符。 |
| [DisplayDocTitle](../../aspose.cells/pdfsaveoptions/displaydoctitle) { get; set; } | 指示窗口的标题栏是否应显示文档标题。 |
| [DrawObjectEventHandler](../../aspose.cells/pdfsaveoptions/drawobjecteventhandler) { get; set; } | 实现该接口，在渲染时获取DrawObject和Bound。 |
| [EmbedStandardWindowsFonts](../../aspose.cells/pdfsaveoptions/embedstandardwindowsfonts) { get; set; } | True 嵌入真字体。 仅影响 ASCII 字符 32-127。 大于 127 的字符代码的字体总是被嵌入的。 PDF/A-1a、PDF/A-1b 标准始终嵌入字体。 默认为真。 |
| [EmfRenderSetting](../../aspose.cells/pdfsaveoptions/emfrendersetting) { get; set; } | 渲染 Emf 图元文件的设置。 |
| [ExportDocumentStructure](../../aspose.cells/pdfsaveoptions/exportdocumentstructure) { get; set; } | 表示是否导出文档结构。 |
| [FontEncoding](../../aspose.cells/pdfsaveoptions/fontencoding) { get; set; } | 获取或设置 pdf 中嵌入的字体编码。 |
| [GridlineType](../../aspose.cells/pdfsaveoptions/gridlinetype) { get; set; } | 获取或设置网格线类型。 |
| [IgnoreError](../../aspose.cells/pdfsaveoptions/ignoreerror) { get; set; } | 表示在渲染时是否需要隐藏错误。 错误可能是形状、图像、图表渲染等方面的错误。 |
| [IsFontSubstitutionCharGranularity](../../aspose.cells/pdfsaveoptions/isfontsubstitutionchargranularity) { get; set; } | 表示当单元格字体不兼容时是否只替换字符的字体。 |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas) { get; set; } | 表示是否在保存文件之前合并条件格式和验证区域。 |
| [OnePagePerSheet](../../aspose.cells/pdfsaveoptions/onepagepersheet) { get; set; } | 如果 OnePagePerSheet 为 true ，则结果中一张表的所有内容将仅输出到一页。 pagesetup 的纸张大小会失效，pagesetup 的其他设置仍然有效。 |
| [OptimizationType](../../aspose.cells/pdfsaveoptions/optimizationtype) { get; set; } | 获取和设置 pdf 优化类型。 |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells/pdfsaveoptions/outputblankpagewhennothingtoprint) { get; set; } | 表示在没有可打印的内容时是否输出空白页。 |
| [PageCount](../../aspose.cells/pdfsaveoptions/pagecount) { get; set; } | 获取或设置要保存的页数。 |
| [PageIndex](../../aspose.cells/pdfsaveoptions/pageindex) { get; set; } | 获取或设置要保存的第一页的从 0 开始的索引。 |
| [PageSavingCallback](../../aspose.cells/pdfsaveoptions/pagesavingcallback) { get; set; } | 控制/指示页面保存过程的进度。 |
| [PdfCompression](../../aspose.cells/pdfsaveoptions/pdfcompression) { get; set; } | 表示压缩算法 |
| [PrintingPageType](../../aspose.cells/pdfsaveoptions/printingpagetype) { get; set; } | 指示不打印哪些页面。 |
| [Producer](../../aspose.cells/pdfsaveoptions/producer) { get; set; } | 获取和设置生成的 pdf 文档的生产者。 |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache) { get; set; } | 表示是否刷新图表缓存数据 |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat) { get; } | 获取保存文件格式。 |
| [SecurityOptions](../../aspose.cells/pdfsaveoptions/securityoptions) { get; set; } | 当 xls2pdf 结果需要安全性时，设置此选项。 |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames) { get; set; } | 表示是否在保存文件之前对外部定义的名称进行排序。 |
| [SortNames](../../aspose.cells/saveoptions/sortnames) { get; set; } | 表示是否在保存文件之前对定义的名称进行排序。 |
| [TextCrossType](../../aspose.cells/pdfsaveoptions/textcrosstype) { get; set; } | 获取或设置文本宽度大于单元格宽度时显示的文本类型。 |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart) { get; set; } | 表示是否更新智能艺术设置。 默认值为假。 |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas) { get; set; } | 表示是否在保存文件之前验证合并的单元格。 |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback) { get; set; } | 获取或设置警告回调。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [SetImageResample](../../aspose.cells/pdfsaveoptions/setimageresample)(int, int) | 设置重新采样图像和 jpeg 质量的所需 PPI（每英寸像素）。 所有图像都将转换为具有指定质量设置的 JPEG， 并且大于指定 PPI（每英寸像素数）的图像将被重新采样。 |

### 也可以看看

* class [SaveOptions](../saveoptions)
* 命名空间 [Aspose.Cells](../../aspose.cells)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
