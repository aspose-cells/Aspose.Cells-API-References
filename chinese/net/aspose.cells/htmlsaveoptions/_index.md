---
title: HtmlSaveOptions
second_title: Aspose.Cells for .NET API 参考
description: 表示保存 html 文件的选项
type: docs
weight: 3740
url: /zh/net/aspose.cells/htmlsaveoptions/
---
## HtmlSaveOptions class

表示保存 html 文件的选项。

```csharp
public class HtmlSaveOptions : SaveOptions
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions#constructor)() | 创建用于保存 html 文件的选项。 |
| [HtmlSaveOptions](htmlsaveoptions#constructor_1)(SaveFormat) | 创建保存 htm 文件的选项。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [AddTooltipText](../../aspose.cells/htmlsaveoptions/addtooltiptext) { get; set; } | 表示数据不能完全显示时是否添加tooltip文本。 默认值为false。 |
| [AttachedFilesDirectory](../../aspose.cells/htmlsaveoptions/attachedfilesdirectory) { get; set; } | 附件要保存到的目录。 仅用于保存到html流。 |
| [AttachedFilesUrlPrefix](../../aspose.cells/htmlsaveoptions/attachedfilesurlprefix) { get; set; } | 指定html文件中图片等附件的Url前缀 仅用于保存到html流 |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder) { get; set; } | 缓存的文件夹是用来存放一些大数据的。 |
| [CellCssPrefix](../../aspose.cells/htmlsaveoptions/cellcssprefix) { get; set; } | 获取和设置css名称的前缀，默认值为""。 |
| [ClearData](../../aspose.cells/saveoptions/cleardata) { get; set; } | 保存文件后使工作簿为空。 |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory) { get; set; } | 如果为true且目录不存在，会在保存文件前自动创建目录。 |
| [DefaultFontName](../../aspose.cells/htmlsaveoptions/defaultfontname) { get; set; } | 指定导出html的默认字体名称，当style的字体不存在时使用默认字体， 如果该属性为空，Aspose.Cells将使用与原始字体同族的通用字体， 默认值为空。 |
| [DisableDownlevelRevealedComments](../../aspose.cells/htmlsaveoptions/disabledownlevelrevealedcomments) { get; set; } | 表示在将文件导出为html时是否禁用Downlevel-revealed条件注释，默认值为false。 |
| [Encoding](../../aspose.cells/htmlsaveoptions/encoding) { get; set; } | 如果未设置，则使用 Encoding.UTF8 作为默认编码类型。 |
| [ExcludeUnusedStyles](../../aspose.cells/htmlsaveoptions/excludeunusedstyles) { get; set; } | 表示是否排除未使用的样式。 对于生成的html文件，排除未使用的样式可以使文件体积更小 不影响视觉效果。所以该属性的默认值为true。 如果用户需要为生成的html保留工作簿中的所有样式（比如user 需要稍后从生成的html恢复工作簿的场景），请将该属性设置为false . |
| [ExportActiveWorksheetOnly](../../aspose.cells/htmlsaveoptions/exportactiveworksheetonly) { get; set; } | 表示是否将整个工作簿导出到 html 文件。 |
| [ExportArea](../../aspose.cells/htmlsaveoptions/exportarea) { get; set; } | 获取或设置当前活动Worksheet的导出CellArea |
| [ExportBogusRowData](../../aspose.cells/htmlsaveoptions/exportbogusrowdata) { get; set; } | 表示是否导出假底行数据。默认值为true。如果要导入html或mht文件 到excel，请保持默认值。 |
| [ExportCellCoordinate](../../aspose.cells/htmlsaveoptions/exportcellcoordinate) { get; set; } | 表示将文件保存为html时是否导出非空白单元格的excel坐标。默认值为false。 如果要将输出的html导入excel，请保持默认值。 |
| [ExportDataOptions](../../aspose.cells/htmlsaveoptions/exportdataoptions) { get; set; } | 表示导出html文件数据的规则。默认值为All。 |
| [ExportDocumentProperties](../../aspose.cells/htmlsaveoptions/exportdocumentproperties) { get; set; } | 表示是否导出文档属性。默认值为true。如果要将 html或mht文件导入excel，请保持默认值。 |
| [ExportExtraHeadings](../../aspose.cells/htmlsaveoptions/exportextraheadings) { get; set; } | 表示当文本长度超过最大显示列时是否导出额外的标题。 默认值为false。如果要将html文件导入excel，请保持默认值。 |
| [ExportFormula](../../aspose.cells/htmlsaveoptions/exportformula) { get; set; } | 表示将文件保存为html时是否导出公式。默认值为true。 如果要将输出的html导入excel，请保持默认值。 |
| [ExportFrameScriptsAndProperties](../../aspose.cells/htmlsaveoptions/exportframescriptsandproperties) { get; set; } | 表示是否导出框架脚本和文档属性。默认值为true。如果要导入html或mht文件 到excel，请保持默认值。 |
| [ExportGridLines](../../aspose.cells/htmlsaveoptions/exportgridlines) { get; set; } | 表示是否导出网格线。默认值为false。 |
| [ExportHiddenWorksheet](../../aspose.cells/htmlsaveoptions/exporthiddenworksheet) { get; set; } | 表示是否导出隐藏的工作表内容。默认值为true。 |
| [ExportImagesAsBase64](../../aspose.cells/htmlsaveoptions/exportimagesasbase64) { get; set; } | 指定图像是否以 Base64 格式保存为 HTML、MHTML 或 EPUB。 |
| [ExportPageFooters](../../aspose.cells/htmlsaveoptions/exportpagefooters) { get; set; } | 表示是否导出页眉。 |
| [ExportPageHeaders](../../aspose.cells/htmlsaveoptions/exportpageheaders) { get; set; } | 表示是否导出页眉。 |
| [ExportPrintAreaOnly](../../aspose.cells/htmlsaveoptions/exportprintareaonly) { get; set; } | 表示是否仅将打印区域导出为 html 文件。默认值为假。 |
| [ExportRowColumnHeadings](../../aspose.cells/htmlsaveoptions/exportrowcolumnheadings) { get; set; } | 表示保存到 HTML 文件时是否导出工作表的行和列标题。 |
| [ExportSimilarBorderStyle](../../aspose.cells/htmlsaveoptions/exportsimilarborderstyle) { get; set; } | 表示浏览器不支持边框样式时是否导出相似的边框样式。 如果要导入html或mht文件到excel，请保持默认值。 默认值为false。 |
| [ExportSingleTab](../../aspose.cells/htmlsaveoptions/exportsingletab) { get; set; } | 表示文件只有一个工作表时是否导出单个选项卡。 默认值为false。 |
| [ExportWorkbookProperties](../../aspose.cells/htmlsaveoptions/exportworkbookproperties) { get; set; } | 表示是否导出工作簿属性。默认值为true。如果要将 html或mht文件导入excel，请保持默认值。 |
| [ExportWorksheetCSSSeparately](../../aspose.cells/htmlsaveoptions/exportworksheetcssseparately) { get; set; } | 表示是否单独导出工作表css。默认值为false。 |
| [ExportWorksheetProperties](../../aspose.cells/htmlsaveoptions/exportworksheetproperties) { get; set; } | 表示是否导出工作表属性。默认值为true。如果要将 html或mht文件导入excel，请保持默认值。 |
| [FilePathProvider](../../aspose.cells/htmlsaveoptions/filepathprovider) { get; set; } | 获取或设置 IFilePathProvider 用于单独将 Worksheet 导出为 html。 |
| [HiddenColDisplayType](../../aspose.cells/htmlsaveoptions/hiddencoldisplaytype) { get; set; } | excel中隐藏的列（该列的宽度为0），保存成html格式之前， 如果HtmlHiddenColDisplayType为“Remove”，隐藏的列不输出， 如果值为“Hidden”，该列将已输出，但已隐藏，默认值为“隐藏” |
| [HiddenRowDisplayType](../../aspose.cells/htmlsaveoptions/hiddenrowdisplaytype) { get; set; } | excel中隐藏的行（该行的高度为0），保存为html格式之前， 如果HtmlHiddenRowDisplayType为“删除”，隐藏的行不会输出， 如果值为“隐藏”，该行将已输出，但已隐藏，默认值为“隐藏” |
| [HtmlCrossStringType](../../aspose.cells/htmlsaveoptions/htmlcrossstringtype) { get; set; } | 表示在将Excel文件保存为html格式时，是否会像MS Excel一样显示跨单元字符串。 默认值为Default，所以对于跨单元字符串，html和MS Excel没有什么区别由 Aspose.Cells 和 MS Excel 创建的文件。 但是创建大型 html 文件的性能，将值设置为 Cross 将比将其设置为 Default 或 Fit2Cell. 快几倍 |
| [IgnoreInvisibleShapes](../../aspose.cells/htmlsaveoptions/ignoreinvisibleshapes) { get; set; } | 表示是否导出那些不可见的形状 |
| [ImageOptions](../../aspose.cells/htmlsaveoptions/imageoptions) { get; } | 导出前获取 ImageOrPrintOptions 对象 |
| [ImageScalable](../../aspose.cells/htmlsaveoptions/imagescalable) { get; set; } | 表示是否使用可缩放单位来描述图像宽度 在使用可缩放单位描述列宽时。 默认值为true。 |
| [IsExpImageToTempDir](../../aspose.cells/htmlsaveoptions/isexpimagetotempdir) { get; set; } | 表示是否将图片文件导出到临时目录。 仅用于保存到html流。 |
| [IsExportComments](../../aspose.cells/htmlsaveoptions/isexportcomments) { get; set; } | 表示是否在将文件保存为html时导出注释，默认值为false。 |
| [IsFullPathLink](../../aspose.cells/htmlsaveoptions/isfullpathlink) { get; set; } | 表示sheet00x.htm、filelist.xml和tabstrip.htm中是否使用全路径链接。 默认值为false。 |
| [LinkTargetType](../../aspose.cells/htmlsaveoptions/linktargettype) { get; set; } | 表示&lt;a&gt;链接中目标属性的类型，默认值为HtmlLinkTargetType.Parent. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas) { get; set; } | 表示是否在保存文件之前合并条件格式和验证区域。 |
| [MergeEmptyTdForcely](../../aspose.cells/htmlsaveoptions/mergeemptytdforcely) { get; set; } | 表示将文件导出为html时是否强制合并空的TD元素。 将值设置为true后，html文件的大小将显着减小。默认值为假。 如果要将html文件导入excel或将文件保存为html时导出完美的网格线， 请保持默认值。 |
| [PageTitle](../../aspose.cells/htmlsaveoptions/pagetitle) { get; set; } | html页面的标题。 仅用于保存到html流。 |
| [ParseHtmlTagInCell](../../aspose.cells/htmlsaveoptions/parsehtmltagincell) { get; set; } | 解析单元格中的 html 标签，例如，作为单元格值，或作为 html 标记，默认为 true |
| [PresentationPreference](../../aspose.cells/htmlsaveoptions/presentationpreference) { get; set; } | 表示html或mht文件是否为演示偏好。默认值为false。如果您想获得 更漂亮的演示，请将值设置为true。 |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache) { get; set; } | 表示是否刷新图表缓存数据 |
| [SaveAsSingleFile](../../aspose.cells/htmlsaveoptions/saveassinglefile) { get; set; } | 表示是否将html保存为单个文件。 默认值为false。 |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat) { get; } | 获取保存文件格式。 |
| [ShowAllSheets](../../aspose.cells/htmlsaveoptions/showallsheets) { get; set; } | 表示保存为单个 html 文件时是否显示所有工作表。 |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames) { get; set; } | 表示是否在保存文件之前对外部定义的名称进行排序。 |
| [SortNames](../../aspose.cells/saveoptions/sortnames) { get; set; } | 表示是否在保存文件之前对定义的名称进行排序。 |
| [StreamProvider](../../aspose.cells/htmlsaveoptions/streamprovider) { get; set; } | 获取或设置用于导出对象的 IStreamProvider。 |
| [TableCssId](../../aspose.cells/htmlsaveoptions/tablecssid) { get; set; } | 获取和设置类型css名称的前缀，如tr,col,td等，它们包含在具有特定TableCssId属性的表元素 中。默认值为 "". |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart) { get; set; } | 表示是否更新智能艺术设置。 默认值为false。 |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas) { get; set; } | 表示是否在保存文件之前验证合并的单元格。 |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback) { get; set; } | 获取或设置警告回调。 |
| [WidthScalable](../../aspose.cells/htmlsaveoptions/widthscalable) { get; set; } | 表示将文件导出为html时是否使用可缩放单位来描述列宽。 默认值为false。 |
| [WorksheetScalable](../../aspose.cells/htmlsaveoptions/worksheetscalable) { get; set; } | 表示将文件保存为html时，是否通过工作表缩放级别放大或缩小html，默认值为false。 |

### 也可以看看

* class [SaveOptions](../saveoptions)
* 命名空间 [Aspose.Cells](../../aspose.cells)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
