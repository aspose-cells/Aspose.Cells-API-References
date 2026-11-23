---
title: "类 EbookSaveOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Saving.EbookSaveOptions 类。表示用于保存电子书文件的选项"
type: docs
url: /zh/net/aspose.cells.saving/ebooksaveoptions/
---
## EbookSaveOptions class

表示用于保存电子书文件的选项。

```csharp
public class EbookSaveOptions : HtmlSaveOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [EbookSaveOptions](ebooksaveoptions/#constructor)() | 创建用于保存电子书文件的选项。 |
| [EbookSaveOptions](ebooksaveoptions/#constructor_1)(SaveFormat) | 创建用于保存电子书文件的选项。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [AddGenericFont](../../aspose.cells/htmlsaveoptions/addgenericfont/) { get; set; } | 指示是否向 CSS font-family 添加通用字体。默认值为 true（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [AddTooltipText](../../aspose.cells/htmlsaveoptions/addtooltiptext/) { get; set; } | 指示在数据无法完整显示时是否添加工具提示文本。默认值为 false。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [AttachedFilesDirectory](../../aspose.cells/htmlsaveoptions/attachedfilesdirectory/) { get; set; } | 附加文件将保存到的目录。仅用于保存为 html 流。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [AttachedFilesUrlPrefix](../../aspose.cells/htmlsaveoptions/attachedfilesurlprefix/) { get; set; } | 指定附加文件（如 html 文件中的图像）的 Url 前缀。仅用于保存为 html 流。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | 用于临时文件的文件夹，可能用作数据缓存。（继承自 [`SaveOptions`](../../aspose.cells/saveoptions/)。） |
| [CalculateFormula](../../aspose.cells/htmlsaveoptions/calculateformula/) { get; set; } | 指示是否在保存 html 文件前计算公式。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [CellCssPrefix](../../aspose.cells/htmlsaveoptions/cellcssprefix/) { get; set; } | 获取和设置 css 名称的前缀，默认值为 ""。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [CellNameAttribute](../../aspose.cells/htmlsaveoptions/cellnameattribute/) { get; set; } | 指定用于写入 CellName 的属性。（例如，如果值为 "id"，则单元格 "A1" 的输出将是：&lt;td id='A1'&gt;）。默认值为 null。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | 是否在用户修改单元格相关对象时检查 Excel 文件的限制。例如，Excel 不允许输入超过 32K 的字符串值。当输入的值超过 32K 时，将被截断。（继承自 [`SaveOptions`](../../aspose.cells/saveoptions/)。） |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | 在保存文件后使工作簿为空。（继承自 [`SaveOptions`](../../aspose.cells/saveoptions/)。） |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | 如果为 true 且目录不存在，则在保存文件之前会自动创建该目录。（继承自 [`SaveOptions`](../../aspose.cells/saveoptions/)。） |
| [CssStyles](../../aspose.cells/htmlsaveoptions/cssstyles/) { get; set; } | 获取或设置格式化程序的附加 css 样式。仅在 [`SaveAsSingleFile`](../../aspose.cells/htmlsaveoptions/saveassinglefile/) 为 True 时有效。CssStyles="body { padding: 5px }"；（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [DataBarRenderMode](../../aspose.cells/htmlsaveoptions/databarrendermode/) { get; set; } | 表示在将 Excel 文件转换为 html 文件时渲染 DataBar 的模式。默认值为 BackgroundColor。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [DefaultFontName](../../aspose.cells/htmlsaveoptions/defaultfontname/) { get; set; } | 指定导出 html 的默认字体名称，当样式的字体不存在时将使用默认字体。如果此属性为 null，Aspose.Cells 将使用与原始字体同族的通用字体，默认值为 null。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [DisableCss](../../aspose.cells/htmlsaveoptions/disablecss/) { get; set; } | 指示是否仅应用内联样式，而不依赖 CSS。默认值为 false。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [DisableDownlevelRevealedComments](../../aspose.cells/htmlsaveoptions/disabledownlevelrevealedcomments/) { get; set; } | 指示在导出文件为 html 时是否禁用 Downlevel-revealed 条件注释，默认值为 false。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [EmbeddedFontType](../../aspose.cells/htmlsaveoptions/embeddedfonttype/) { get; set; } | 获取或设置嵌入字体文件到 html 文件的类型。默认值为 None，表示不在 html 中嵌入任何字体。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [EnableCssCustomProperties](../../aspose.cells/htmlsaveoptions/enablecsscustomproperties/) { get; set; } | 通过使用 CSS 自定义属性优化 html 输出。例如，对于同一 base64 图像出现多次的情况，使用自定义属性只需保存一次图像数据，从而提升生成的 html 性能。默认值为 false。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [EncodeEntityAsCode](../../aspose.cells/htmlsaveoptions/encodeentityascode/) { get; set; } | 指示是否将 html 字符实体替换为十进制代码。（例如 \"&amp;nbsp;\" 被替换为 \"&amp;#160;\"）。默认值为 false。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [Encoding](../../aspose.cells/htmlsaveoptions/encoding/) { get; set; } | 如果未设置，则使用 Encoding.UTF8 作为默认编码类型。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | 指示在保存为 .xls 文件时是否加密文档属性。默认值为 true。（继承自 [`SaveOptions`](../../aspose.cells/saveoptions/)。） |
| [ExcludeUnusedStyles](../../aspose.cells/htmlsaveoptions/excludeunusedstyles/) { get; set; } | 指示是否排除未使用的样式。对于生成的 html 文件，排除未使用的样式可以在不影响视觉效果的情况下减小文件大小。因此此属性的默认值为 true。如果用户需要在工作簿中保留所有样式以用于生成的 html（例如用户稍后需要从生成的 html 恢复工作簿的场景），请将此属性设置为 false。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [ExportActiveWorksheetOnly](../../aspose.cells/htmlsaveoptions/exportactiveworksheetonly/) { get; set; } | 指示是否仅导出活动工作表到 html 文件。如果为 true，则仅导出活动工作表；如果为 false，则导出整个工作簿。默认值为 false。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [ExportArea](../../aspose.cells/htmlsaveoptions/exportarea/) { get; set; } | 获取或设置当前活动工作表的导出 CellArea。如果设置此属性，当前活动工作表的打印区域将被省略。保存文件为 html 时仅导出指定区域。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [ExportBogusRowData](../../aspose.cells/htmlsaveoptions/exportbogusrowdata/) { get; set; } | 指示是否导出虚假的底部行数据。默认值为 true。如果希望将 html 或 mht 文件导入到 excel，请保持默认值。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [ExportCellCoordinate](../../aspose.cells/htmlsaveoptions/exportcellcoordinate/) { get; set; } | 指示在保存文件为 html 时是否导出非空单元格的 Excel 坐标。默认值为 false。如果希望将输出的 html 导入到 excel，请保持默认值。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [ExportCommentsType](../../aspose.cells/htmlsaveoptions/exportcommentstype/) { get; set; } | 表示导出注释到 html 文件的类型。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [ExportDataOptions](../../aspose.cells/htmlsaveoptions/exportdataoptions/) { get; set; } | 指示导出 html 文件数据的规则。默认值为 All。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [ExportDocumentProperties](../../aspose.cells/htmlsaveoptions/exportdocumentproperties/) { get; set; } | 指示是否导出文档属性。默认值为 true。如果希望将 html 或 mht 文件导入到 excel，请保持默认值。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [ExportExtraHeadings](../../aspose.cells/htmlsaveoptions/exportextraheadings/) { get; set; } | 指示当文本长度超过最大显示列时是否导出额外的标题。默认值为 false。如果希望将 html 文件导入到 excel，请保持默认值。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [ExportFormula](../../aspose.cells/htmlsaveoptions/exportformula/) { get; set; } | 指示在保存文件为 html 时是否导出公式。默认值为 true。如果希望将输出的 html 导入到 excel，请保持默认值。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [ExportFrameScriptsAndProperties](../../aspose.cells/htmlsaveoptions/exportframescriptsandproperties/) { get; set; } | 指示是否导出框架脚本和文档属性。默认值为 true。如果希望将 html 或 mht 文件导入到 excel，请保持默认值。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [ExportGridLines](../../aspose.cells/htmlsaveoptions/exportgridlines/) { get; set; } | 指示是否导出网格线。默认值为 false。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [ExportHeadings](../../aspose.cells/htmlsaveoptions/exportheadings/) { get; set; } | (**Obsolete.**) 指示在保存为 HTML 文件时是否导出工作表的行和列标题。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [ExportHiddenWorksheet](../../aspose.cells/htmlsaveoptions/exporthiddenworksheet/) { get; set; } | 指示是否导出隐藏工作表的内容。默认值为 true。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [ExportImagesAsBase64](../../aspose.cells/htmlsaveoptions/exportimagesasbase64/) { get; set; } | 指定是否将图像以 Base64 格式保存为 HTML、MHTML 或 EPUB。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [ExportNamedRangeAnchors](../../aspose.cells/htmlsaveoptions/exportnamedrangeanchors/) { get; set; } | 指示在保存为 HTML 时是否导出命名范围的锚点元素。默认值为 true。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [ExportObjectListener](../../aspose.cells/htmlsaveoptions/exportobjectlistener/) { get; set; } | (**Obsolete.**) 获取或设置用于导出对象的 ExportObjectListener。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [ExportPageFooters](../../aspose.cells/htmlsaveoptions/exportpagefooters/) { get; set; } | 指示是否导出页面标题。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [ExportPageHeaders](../../aspose.cells/htmlsaveoptions/exportpageheaders/) { get; set; } | 指示是否导出页面标题。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [ExportPrintAreaOnly](../../aspose.cells/htmlsaveoptions/exportprintareaonly/) { get; set; } | 指示是否仅导出打印区域到 html 文件。默认值为 false。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [ExportRowColumnHeadings](../../aspose.cells/htmlsaveoptions/exportrowcolumnheadings/) { get; set; } | 指示在保存为 HTML 文件时是否导出工作表的行和列标题。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [ExportSimilarBorderStyle](../../aspose.cells/htmlsaveoptions/exportsimilarborderstyle/) { get; set; } | 指示在浏览器不支持的情况下是否导出相似的边框样式。如果希望将 html 或 mht 文件导入到 excel，请保持默认值。默认值为 false。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [ExportSingleTab](../../aspose.cells/htmlsaveoptions/exportsingletab/) { get; set; } | 指示当文件仅包含一个工作表时是否导出单个标签页。默认值为 false。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [ExportWorkbookProperties](../../aspose.cells/htmlsaveoptions/exportworkbookproperties/) { get; set; } | 指示是否导出工作簿属性。默认值为 true。如果要将 html 或 mht 文件导入 Excel，请保持默认值。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [ExportWorksheetCSSSeparately](../../aspose.cells/htmlsaveoptions/exportworksheetcssseparately/) { get; set; } | 指示是否单独导出工作表 CSS。默认值为 false。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [ExportWorksheetProperties](../../aspose.cells/htmlsaveoptions/exportworksheetproperties/) { get; set; } | 指示是否导出工作表属性。默认值为 true。如果要将 html 或 mht 文件导入 Excel，请保持默认值。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [FilePathProvider](../../aspose.cells/htmlsaveoptions/filepathprovider/) { get; set; } | 获取或设置用于单独将工作表导出为 html 的 IFilePathProvider。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [FormatDataIgnoreColumnWidth](../../aspose.cells/htmlsaveoptions/formatdataignorecolumnwidth/) { get; set; } | 指示当单元格内容溢出列时是否显示完整的格式化数据。如果为 true，则忽略列宽，导出完整的单元格数据。如果为 false，则数据的导出方式与 Excel 相同。默认值为 false。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [HiddenColDisplayType](../../aspose.cells/htmlsaveoptions/hiddencoldisplaytype/) { get; set; } | Excel 中的隐藏列（该列宽度为 0），在保存为 html 格式之前，如果 HtmlHiddenColDisplayType 为 \"Remove\"，则隐藏列不会被输出；如果值为 \"Hidden\"，列会被输出但保持隐藏，默认值为 \"Hidden\”。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [HiddenRowDisplayType](../../aspose.cells/htmlsaveoptions/hiddenrowdisplaytype/) { get; set; } | Excel 中的隐藏行（该行高度为 0），在保存为 html 格式之前，如果 HtmlHiddenRowDisplayType 为 \"Remove\"，则隐藏行不会被输出；如果值为 \"Hidden\"，行会被输出但保持隐藏，默认值为 \"Hidden\”。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [HideOverflowWrappedText](../../aspose.cells/htmlsaveoptions/hideoverflowwrappedtext/) { get; set; } | 指示当单元格格式设置为自动换行时是否隐藏溢出文本。默认值为 false。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [HtmlCrossStringType](../../aspose.cells/htmlsaveoptions/htmlcrossstringtype/) { get; set; } | 指示在将 Excel 文件保存为 html 格式时，跨单元格的字符串是否以与 MS Excel 相同的方式显示。默认值为 Default，因此对于跨单元格的字符串，Aspose.Cells 创建的 html 文件与 MS Excel 的差别很小。但在生成大型 html 文件时，将该值设为 Cross 的性能会比设为 Default 或 Fit2Cell 快数倍。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [HtmlVersion](../../aspose.cells/htmlsaveoptions/htmlversion/) { get; set; } | 指定保存为 HTML 格式时应使用的 HTML 标准版本。默认值为 HtmlVersion.Default。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [IgnoreInvisibleShapes](../../aspose.cells/htmlsaveoptions/ignoreinvisibleshapes/) { get; set; } | 指示是否导出不可见的形状。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [ImageOptions](../../aspose.cells/htmlsaveoptions/imageoptions/) { get; } | 在导出之前获取 ImageOrPrintOptions 对象。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [ImageScalable](../../aspose.cells/htmlsaveoptions/imagescalable/) { get; set; } | 指示在使用可伸缩单位描述列宽时，是否使用可伸缩单位描述图像宽度。默认值为 true。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [IsBorderCollapsed](../../aspose.cells/htmlsaveoptions/isbordercollapsed/) { get; set; } | 指示表格边框是否折叠。默认值为 true。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [IsExpImageToTempDir](../../aspose.cells/htmlsaveoptions/isexpimagetotempdir/) { get; set; } | 指示是否将图像文件导出到临时目录。仅用于保存为 html 流。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [IsExportComments](../../aspose.cells/htmlsaveoptions/isexportcomments/) { get; set; } | 指示在将文件保存为 html 时是否导出批注，默认值为 false。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [IsFullPathLink](../../aspose.cells/htmlsaveoptions/isfullpathlink/) { get; set; } | 指示在 sheet00x.htm、filelist.xml 和 tabstrip.htm 中是否使用完整路径链接。默认值为 false。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [IsIECompatible](../../aspose.cells/htmlsaveoptions/isiecompatible/) { get; set; } | 指示输出的 HTML 是否兼容 IE 浏览器。默认值为 false。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [IsJsBrowserCompatible](../../aspose.cells/htmlsaveoptions/isjsbrowsercompatible/) { get; set; } | 指示 JavaScript 是否兼容不支持 JavaScript 的浏览器。默认值为 true。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [IsMobileCompatible](../../aspose.cells/htmlsaveoptions/ismobilecompatible/) { get; set; } | 指示输出的 HTML 是否兼容移动设备。默认值为 false。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [LayoutMode](../../aspose.cells/htmlsaveoptions/layoutmode/) { get; set; } | 获取或设置保存为 HTML 时的布局模式。默认值为 Normal。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [LinkTargetType](../../aspose.cells/htmlsaveoptions/linktargettype/) { get; set; } | 指示 `<a>` 链接中 target 属性的类型。默认值为 HtmlLinkTargetType.Parent。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | 指示在保存文件之前是否合并条件格式和数据验证的区域。（继承自 [`SaveOptions`](../../aspose.cells/saveoptions/)。） |
| [MergeEmptyTdForcely](../../aspose.cells/htmlsaveoptions/mergeemptytdforcely/) { get; set; } | (**Obsolete.**) 指示在导出文件为 html 时是否强制合并空的 TD 元素。将该值设为 true 后，html 文件大小将显著减小。默认值为 false。如果希望将 html 文件导入 Excel 或在保存为 html 时导出完整的网格线，请保持默认值。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [MergeEmptyTdType](../../aspose.cells/htmlsaveoptions/mergeemptytdtype/) { get; set; } | 合并连续空单元格（空 td 元素）的选项。默认值为 MergeEmptyTdType.Default。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [OfficeMathOutputMode](../../aspose.cells/htmlsaveoptions/officemathoutputmode/) { get; set; } | 指示 OfficeMath 对象导出为 HTML 的方式，默认值为 Image。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [PageTitle](../../aspose.cells/htmlsaveoptions/pagetitle/) { get; set; } | HTML 页面标题。仅用于保存为 HTML 流。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [ParseHtmlTagInCell](../../aspose.cells/htmlsaveoptions/parsehtmltagincell/) { get; set; } | 指示单元格中的 HTML 标记（例如 `<div></div>`）是应解析为单元格值还是保持原样。默认值为 true。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [PresentationPreference](../../aspose.cells/htmlsaveoptions/presentationpreference/) { get; set; } | 指示 HTML 或 MHT 文件是否为呈现首选项。默认值为 false。如果希望获得更美观的呈现，请将该值设为 true。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | 指示是否缓存图表的最新数据。（继承自 [`SaveOptions`](../../aspose.cells/saveoptions/)。） |
| [SaveAsSingleFile](../../aspose.cells/htmlsaveoptions/saveassinglefile/) { get; set; } | 指示是否将 HTML 保存为单个文件。默认值为 false。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | 获取保存文件的格式。（继承自 [`SaveOptions`](../../aspose.cells/saveoptions/)。） |
| [SheetSet](../../aspose.cells/htmlsaveoptions/sheetset/) { get; set; } | 获取或设置要渲染的工作表。默认是工作簿中所有可见的工作表：[`Visible`](../../aspose.cells.rendering/sheetset/visible/).（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [ShowAllSheets](../../aspose.cells/htmlsaveoptions/showallsheets/) { get; set; } | 指示在保存为单个 HTML 文件时是否显示所有工作表。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | 指示在保存文件之前是否对外部已定义的名称进行排序。（继承自 [`SaveOptions`](../../aspose.cells/saveoptions/)。） |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | 指示在保存文件之前是否对已定义的名称进行排序。（继承自 [`SaveOptions`](../../aspose.cells/saveoptions/)。） |
| [SpaceMode](../../aspose.cells/htmlsaveoptions/spacemode/) { get; set; } | 指示在 HTML 输出中空格的渲染方式。此选项目前仅适用于数字格式（例如会计格式）。默认值为 Css。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [StreamProvider](../../aspose.cells/htmlsaveoptions/streamprovider/) { get; set; } | 获取或设置用于导出对象的 IStreamProvider。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [TableCssId](../../aspose.cells/htmlsaveoptions/tablecssid/) { get; set; } | 获取并设置类型 CSS 名称的前缀，如 tr、col、td 等，它们位于具有特定 TableCssId 属性的 table 元素中。默认值为 ""。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | 指示是否更新 Smart Art 设置。默认值为 false。（继承自 [`SaveOptions`](../../aspose.cells/saveoptions/)。） |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | 指示是否在保存文件之前验证合并单元格。（继承自 [`SaveOptions`](../../aspose.cells/saveoptions/)。） |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | 获取或设置警告回调。（继承自 [`SaveOptions`](../../aspose.cells/saveoptions/)。） |
| [WidthScalable](../../aspose.cells/htmlsaveoptions/widthscalable/) { get; set; } | 指示是否以比例单位导出列宽到 HTML。默认值为 false。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |
| [WorksheetScalable](../../aspose.cells/htmlsaveoptions/worksheetscalable/) { get; set; } | 指示在将文件保存为 HTML 时，是否通过工作表缩放级别对 HTML 进行放大或缩小，默认值为 false。（继承自 [`HtmlSaveOptions`](../../aspose.cells/htmlsaveoptions/)。） |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class EbookSaveOptionsDemo
    {
        public static void EbookSaveOptionsExample()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue("Hello World");

            // 创建 EbookSaveOptions 的实例
            EbookSaveOptions saveOptions = new EbookSaveOptions();

            // 设置属性
            saveOptions.IgnoreInvisibleShapes = true;
            saveOptions.PageTitle = "Sample Page Title";
            saveOptions.AttachedFilesDirectory = "attached_files";
            saveOptions.AttachedFilesUrlPrefix = "http://example.com/files/";
            saveOptions.DefaultFontName = "Arial";
            saveOptions.AddGenericFont = true;
            saveOptions.WorksheetScalable = false;
            saveOptions.IsExportComments = false;
            saveOptions.ExportCommentsType = PrintCommentsType.PrintNoComments;
            saveOptions.DisableDownlevelRevealedComments = false;
            saveOptions.IsExpImageToTempDir = false;
            saveOptions.ImageScalable = true;
            saveOptions.WidthScalable = false;
            saveOptions.ExportSingleTab = false;
            saveOptions.ExportImagesAsBase64 = false;
            saveOptions.ExportActiveWorksheetOnly = false;
            saveOptions.ExportPrintAreaOnly = false;
            saveOptions.ExportArea = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            saveOptions.ParseHtmlTagInCell = true;
            saveOptions.HtmlCrossStringType = HtmlCrossType.Default;
            saveOptions.HiddenColDisplayType = HtmlHiddenColDisplayType.Hidden;
            saveOptions.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden;
            saveOptions.Encoding = System.Text.Encoding.UTF8;
            saveOptions.SaveAsSingleFile = false;
            saveOptions.ShowAllSheets = true;
            saveOptions.ExportPageHeaders = true;
            saveOptions.ExportPageFooters = true;
            saveOptions.ExportHiddenWorksheet = true;
            saveOptions.PresentationPreference = false;
            saveOptions.CellCssPrefix = "cell_";
            saveOptions.TableCssId = "table_";
            saveOptions.IsFullPathLink = false;
            saveOptions.ExportWorksheetCSSSeparately = false;
            saveOptions.ExportSimilarBorderStyle = false;
            saveOptions.MergeEmptyTdForcely = false;
            saveOptions.MergeEmptyTdType = MergeEmptyTdType.Default;
            saveOptions.ExportCellCoordinate = false;
            saveOptions.ExportExtraHeadings = false;
            saveOptions.ExportHeadings = true;
            saveOptions.ExportRowColumnHeadings = true;
            saveOptions.ExportFormula = true;
            saveOptions.AddTooltipText = false;
            saveOptions.ExportGridLines = false;
            saveOptions.ExportBogusRowData = true;
            saveOptions.ExcludeUnusedStyles = true;
            saveOptions.ExportDocumentProperties = true;
            saveOptions.ExportWorksheetProperties = true;
            saveOptions.ExportWorkbookProperties = true;
            saveOptions.ExportFrameScriptsAndProperties = true;
            saveOptions.ExportDataOptions = HtmlExportDataOptions.All;
            saveOptions.LinkTargetType = HtmlLinkTargetType.Parent;
            saveOptions.IsIECompatible = false;
            saveOptions.FormatDataIgnoreColumnWidth = false;
            saveOptions.CalculateFormula = true;
            saveOptions.IsJsBrowserCompatible = true;
            saveOptions.IsMobileCompatible = false;
            saveOptions.CssStyles = "body { padding: 5px }";
            saveOptions.HideOverflowWrappedText = false;
            saveOptions.IsBorderCollapsed = true;
            saveOptions.ClearData = true;
            saveOptions.CachedFileFolder = "cache";
            saveOptions.ValidateMergedAreas = true;
            saveOptions.MergeAreas = true;
            saveOptions.SortNames = true;
            saveOptions.SortExternalNames = true;
            saveOptions.RefreshChartCache = true;
            saveOptions.WarningCallback = null;
            saveOptions.UpdateSmartArt = true;

            // 使用指定的选项将工作簿保存为 HTML 文件
            workbook.Save("EbookSaveOptionsExample.html", saveOptions);

            return;
        }
    }
}
```

### 另请参见

* class [HtmlSaveOptions](../../aspose.cells/htmlsaveoptions/)
* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


