---
title: "EbookSaveOptions 类"
linktitle: "EbookSaveOptions"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "EbookSaveOptions 类。封装在 Go 中表示 ebooksaveoptions 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/ebooksaveoptions/
---

## EbookSaveOptions class

表示保存电子书文件的选项。

```go

type EbookSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewEbookSaveOptions](./newebooksaveoptions/) | 创建保存电子书文件的选项。 |
| [NewEbookSaveOptions_SaveFormat](./newebooksaveoptions_saveformat/) | 创建保存电子书文件的选项。 |
| [NewEbookSaveOptions_HtmlSaveOptions](./newebooksaveoptions_htmlsaveoptions/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetIgnoreInvisibleShapes](./getignoreinvisibleshapes/) | 指示是否导出不可见的形状。 |
| [SetIgnoreInvisibleShapes](./setignoreinvisibleshapes/) | 指示是否导出不可见的形状。 |
| [GetPageTitle](./getpagetitle/) | html 页面标题。仅用于保存为 html 流。 |
| [SetPageTitle](./setpagetitle/) | html 页面标题。仅用于保存为 html 流。 |
| [GetAttachedFilesDirectory](./getattachedfilesdirectory/) | 附加文件将保存到的目录。仅用于保存为 html 流。 |
| [SetAttachedFilesDirectory](./setattachedfilesdirectory/) | 附加文件将保存到的目录。仅用于保存为 html 流。 |
| [GetAttachedFilesUrlPrefix](./getattachedfilesurlprefix/) | 指定 html 文件中附加文件（如图像）的 Url 前缀。仅用于保存为 html 流。 |
| [SetAttachedFilesUrlPrefix](./setattachedfilesurlprefix/) | 指定 html 文件中附加文件（如图像）的 Url 前缀。仅用于保存为 html 流。 |
| [GetDefaultFontName](./getdefaultfontname/) | 指定导出 html 时的默认字体名称，当样式的字体不存在时将使用默认字体。如果此属性为 null，Aspose.Cells 将使用与原始字体同族的通用字体，默认值为 null。 |
| [SetDefaultFontName](./setdefaultfontname/) | 指定导出 html 时的默认字体名称，当样式的字体不存在时将使用默认字体。如果此属性为 null，Aspose.Cells 将使用与原始字体同族的通用字体，默认值为 null。 |
| [GetAddGenericFont](./getaddgenericfont/) | 指示是否向 CSS font-family 添加通用字体。默认值为 true。 |
| [SetAddGenericFont](./setaddgenericfont/) | 指示是否向 CSS font-family 添加通用字体。默认值为 true。 |
| [GetWorksheetScalable](./getworksheetscalable/) | 指示在将文件保存为 html 时是否通过工作表缩放级别对 html 进行放大或缩小，默认值为 false。 |
| [SetWorksheetScalable](./setworksheetscalable/) | 指示在将文件保存为 html 时是否通过工作表缩放级别对 html 进行放大或缩小，默认值为 false。 |
| [IsExportComments](./isexportcomments/) | 指示在将文件保存为 html 时是否导出注释，默认值为 false。 |
| [SetIsExportComments](./setisexportcomments/) | 指示在将文件保存为 html 时是否导出注释，默认值为 false。 |
| [GetExportCommentsType](./getexportcommentstype/) | 表示导出注释到 html 文件的类型。 |
| [SetExportCommentsType](./setexportcommentstype/) | 表示导出注释到 html 文件的类型。 |
| [GetDisableDownlevelRevealedComments](./getdisabledownlevelrevealedcomments/) | 指示在导出文件为 html 时是否禁用 Downlevel-revealed 条件注释，默认值为 false。 |
| [SetDisableDownlevelRevealedComments](./setdisabledownlevelrevealedcomments/) | 指示在导出文件为 html 时是否禁用 Downlevel-revealed 条件注释，默认值为 false。 |
| [IsExpImageToTempDir](./isexpimagetotempdir/) | 指示是否将图像文件导出到临时目录。仅用于保存为 html 流。 |
| [SetIsExpImageToTempDir](./setisexpimagetotempdir/) | 指示是否将图像文件导出到临时目录。仅用于保存为 html 流。 |
| [GetImageScalable](./getimagescalable/) | 指示在使用可伸缩单位描述列宽时，是否使用可伸缩单位描述图像宽度。默认值为 true。 |
| [SetImageScalable](./setimagescalable/) | 指示在使用可伸缩单位描述列宽时，是否使用可伸缩单位描述图像宽度。默认值为 true。 |
| [GetWidthScalable](./getwidthscalable/) | 指示是否以比例单位将列宽导出到 html。默认值为 false。 |
| [SetWidthScalable](./setwidthscalable/) | 指示是否以比例单位将列宽导出到 html。默认值为 false。 |
| [GetExportSingleTab](./getexportsingletab/) | 指示当文件仅包含一个工作表时是否导出单个标签页。默认值为 false。 |
| [SetExportSingleTab](./setexportsingletab/) | 指示当文件仅包含一个工作表时是否导出单个标签页。默认值为 false。 |
| [GetExportImagesAsBase64](./getexportimagesasbase64/) | 指定是否将图像以 Base64 格式保存到 HTML、MHTML 或 EPUB。 |
| [SetExportImagesAsBase64](./setexportimagesasbase64/) | 指定是否将图像以 Base64 格式保存到 HTML、MHTML 或 EPUB。 |
| [GetExportActiveWorksheetOnly](./getexportactiveworksheetonly/) | 指示是否仅将活动工作表导出为 html 文件。如果为 true，则仅导出活动工作表；如果为 false，则导出整个工作簿。默认值为 false。 |
| [SetExportActiveWorksheetOnly](./setexportactiveworksheetonly/) | 指示是否仅将活动工作表导出为 html 文件。如果为 true，则仅导出活动工作表；如果为 false，则导出整个工作簿。默认值为 false。 |
| [GetExportPrintAreaOnly](./getexportprintareaonly/) | 指示是否仅导出打印区域到 html 文件。默认值为 false。 |
| [SetExportPrintAreaOnly](./setexportprintareaonly/) | 指示是否仅导出打印区域到 html 文件。默认值为 false。 |
| [GetExportArea](./getexportarea/) | 获取或设置当前活动工作表的导出 CellArea。如果设置此属性，当前活动工作表的打印区域将被省略。保存文件为 html 时仅导出指定区域。 |
| [SetExportArea](./setexportarea/) | 获取或设置当前活动工作表的导出 CellArea。如果设置此属性，当前活动工作表的打印区域将被省略。保存文件为 html 时仅导出指定区域。 |
| [GetParseHtmlTagInCell](./getparsehtmltagincell/) | 指示单元格中的 html 标签（例如 <c>&lt;div&gt;&lt;/div&gt;</c>）是应解析为单元格值还是保持原样。默认值为 true。 |
| [SetParseHtmlTagInCell](./setparsehtmltagincell/) | 指示单元格中的 html 标签（例如 <c>&lt;div&gt;&lt;/div&gt;</c>）是应解析为单元格值还是保持原样。默认值为 true。 |
| [GetHtmlCrossStringType](./gethtmlcrossstringtype/) | 指示在将 Excel 文件保存为 html 格式时，跨单元格字符串是否以与 MS Excel 相同的方式显示。默认值为 Default，因此对于跨单元格字符串，Aspose.Cells 创建的 html 文件与 MS Excel 的差别很小。但在创建大型 html 文件时，将值设为 Cross 的性能会比设为 Default 或 Fit2Cell 快数倍。 |
| [SetHtmlCrossStringType](./sethtmlcrossstringtype/) | 指示在将 Excel 文件保存为 html 格式时，跨单元格字符串是否以与 MS Excel 相同的方式显示。默认值为 Default，因此对于跨单元格字符串，Aspose.Cells 创建的 html 文件与 MS Excel 的差别很小。但在创建大型 html 文件时，将值设为 Cross 的性能会比设为 Default 或 Fit2Cell 快数倍。 |
| [GetHiddenColDisplayType](./gethiddencoldisplaytype/) | Excel 中的隐藏列（该列宽度为 0），在保存为 html 格式之前，如果 HtmlHiddenColDisplayType 为 "Remove"，则隐藏列不会输出；如果值为 "Hidden"，则列会输出但保持隐藏，默认值为 "Hidden"。 |
| [SetHiddenColDisplayType](./sethiddencoldisplaytype/) | Excel 中的隐藏列（该列宽度为 0），在保存为 html 格式之前，如果 HtmlHiddenColDisplayType 为 "Remove"，则隐藏列不会输出；如果值为 "Hidden"，则列会输出但保持隐藏，默认值为 "Hidden"。 |
| [GetHiddenRowDisplayType](./gethiddenrowdisplaytype/) | Excel 中的隐藏行（该行高度为 0），在保存为 html 格式之前，如果 HtmlHiddenRowDisplayType 为 "Remove"，则隐藏行不会输出；如果值为 "Hidden"，则行会输出但保持隐藏，默认值为 "Hidden"。 |
| [SetHiddenRowDisplayType](./sethiddenrowdisplaytype/) | Excel 中的隐藏行（该行高度为 0），在保存为 html 格式之前，如果 HtmlHiddenRowDisplayType 为 "Remove"，则隐藏行不会输出；如果值为 "Hidden"，则行会输出但保持隐藏，默认值为 "Hidden"。 |
| [GetEncoding](./getencoding/) | 如果未设置，则使用 Encoding.UTF8 作为默认编码类型。 |
| [SetEncoding](./setencoding/) | 如果未设置，则使用 Encoding.UTF8 作为默认编码类型。 |
| [GetImageOptions](./getimageoptions/) | 在导出之前获取 ImageOrPrintOptions 对象。 |
| [GetSaveAsSingleFile](./getsaveassinglefile/) | 指示是否将 html 保存为单个文件。默认值为 false。 |
| [SetSaveAsSingleFile](./setsaveassinglefile/) | 指示是否将 html 保存为单个文件。默认值为 false。 |
| [GetShowAllSheets](./getshowallsheets/) | 指示在保存为单个 html 文件时是否显示所有工作表。 |
| [SetShowAllSheets](./setshowallsheets/) | 指示在保存为单个 html 文件时是否显示所有工作表。 |
| [GetExportPageHeaders](./getexportpageheaders/) | 指示是否导出页面标题。 |
| [SetExportPageHeaders](./setexportpageheaders/) | 指示是否导出页面标题。 |
| [GetExportPageFooters](./getexportpagefooters/) | 指示是否导出页面标题。 |
| [SetExportPageFooters](./setexportpagefooters/) | 指示是否导出页面标题。 |
| [GetExportHiddenWorksheet](./getexporthiddenworksheet/) | 指示是否导出隐藏工作表的内容。默认值为 true。 |
| [SetExportHiddenWorksheet](./setexporthiddenworksheet/) | 指示是否导出隐藏工作表的内容。默认值为 true。 |
| [GetPresentationPreference](./getpresentationpreference/) | 指示 html 或 mht 文件是否为首选展示格式。默认值为 false。如果希望获得更美观的展示，请将该值设为 true。 |
| [SetPresentationPreference](./setpresentationpreference/) | 指示 html 或 mht 文件是否为首选展示格式。默认值为 false。如果希望获得更美观的展示，请将该值设为 true。 |
| [GetCellCssPrefix](./getcellcssprefix/) | 获取和设置 css 名称的前缀，默认值为 ""。 |
| [SetCellCssPrefix](./setcellcssprefix/) | 获取和设置 css 名称的前缀，默认值为 ""。 |
| [GetTableCssId](./gettablecssid/) | 获取和设置类型 css 名称（如 tr、col、td 等）的前缀，这些名称位于具有特定 TableCssId 属性的 table 元素中。默认值为 ""。 |
| [SetTableCssId](./settablecssid/) | 获取和设置类型 css 名称（如 tr、col、td 等）的前缀，这些名称位于具有特定 TableCssId 属性的 table 元素中。默认值为 ""。 |
| [IsFullPathLink](./isfullpathlink/) | 指示是否在 sheet00x.htm、filelist.xml 和 tabstrip.htm 中使用完整路径链接。默认值为 false。 |
| [SetIsFullPathLink](./setisfullpathlink/) | 指示是否在 sheet00x.htm、filelist.xml 和 tabstrip.htm 中使用完整路径链接。默认值为 false。 |
| [GetExportWorksheetCSSSeparately](./getexportworksheetcssseparately/) | 指示是否单独导出工作表的 CSS。默认值为 false。 |
| [SetExportWorksheetCSSSeparately](./setexportworksheetcssseparately/) | 指示是否单独导出工作表的 CSS。默认值为 false。 |
| [GetExportSimilarBorderStyle](./getexportsimilarborderstyle/) | 指示在浏览器不支持边框样式时是否导出相似的边框样式。如果希望将 html 或 mht 文件导入 Excel，请保持默认值。默认值为 false。 |
| [SetExportSimilarBorderStyle](./setexportsimilarborderstyle/) | 指示在浏览器不支持边框样式时是否导出相似的边框样式。如果希望将 html 或 mht 文件导入 Excel，请保持默认值。默认值为 false。 |
| [GetMergeEmptyTdType](./getmergeemptytdtype/) | 合并连续空单元格（空 td 元素）的选项。默认值为 MergeEmptyTdType.Default。 |
| [SetMergeEmptyTdType](./setmergeemptytdtype/) | 合并连续空单元格（空 td 元素）的选项。默认值为 MergeEmptyTdType.Default。 |
| [GetExportCellCoordinate](./getexportcellcoordinate/) | 指示在将文件保存为 html 时是否导出非空单元格的 Excel 坐标。默认值为 false。如果希望将输出的 html 导入 Excel，请保持默认值。 |
| [SetExportCellCoordinate](./setexportcellcoordinate/) | 指示在将文件保存为 html 时是否导出非空单元格的 Excel 坐标。默认值为 false。如果希望将输出的 html 导入 Excel，请保持默认值。 |
| [GetExportExtraHeadings](./getexportextraheadings/) | 指示当文本长度超过最大显示列时是否导出额外的标题。默认值为 false。如果希望将 html 文件导入 Excel，请保持默认值。 |
| [SetExportExtraHeadings](./setexportextraheadings/) | 指示当文本长度超过最大显示列时是否导出额外的标题。默认值为 false。如果希望将 html 文件导入 Excel，请保持默认值。 |
| [GetExportRowColumnHeadings](./getexportrowcolumnheadings/) | 指示在保存为 HTML 文件时是否导出工作表的行列标题。 |
| [SetExportRowColumnHeadings](./setexportrowcolumnheadings/) | 指示在保存为 HTML 文件时是否导出工作表的行列标题。 |
| [GetExportFormula](./getexportformula/) | 指示在将文件保存为 html 时是否导出公式。默认值为 true。如果希望将输出的 html 导入 Excel，请保持默认值。 |
| [SetExportFormula](./setexportformula/) | 指示在将文件保存为 html 时是否导出公式。默认值为 true。如果希望将输出的 html 导入 Excel，请保持默认值。 |
| [GetAddTooltipText](./getaddtooltiptext/) | 指示当数据无法完整显示时是否添加工具提示文本。默认值为 false。 |
| [SetAddTooltipText](./setaddtooltiptext/) | 指示当数据无法完整显示时是否添加工具提示文本。默认值为 false。 |
| [GetExportGridLines](./getexportgridlines/) | 指示是否导出网格线。默认值为 false。 |
| [SetExportGridLines](./setexportgridlines/) | 指示是否导出网格线。默认值为 false。 |
| [GetExportBogusRowData](./getexportbogusrowdata/) | 指示是否导出虚假的底部行数据。默认值为 true。如果希望将 html 或 mht 文件导入 Excel，请保持默认值。 |
| [SetExportBogusRowData](./setexportbogusrowdata/) | 指示是否导出虚假的底部行数据。默认值为 true。如果希望将 html 或 mht 文件导入 Excel，请保持默认值。 |
| [GetExcludeUnusedStyles](./getexcludeunusedstyles/) | 指示是否排除未使用的样式。对于生成的 html 文件，排除未使用的样式可以在不影响视觉效果的情况下减小文件大小。因此此属性的默认值为 true。如果用户需要在工作簿中保留所有样式以用于生成的 html（例如用户稍后需要从生成的 html 恢复工作簿的场景），请将此属性设为 false。 |
| [SetExcludeUnusedStyles](./setexcludeunusedstyles/) | 指示是否排除未使用的样式。对于生成的 html 文件，排除未使用的样式可以在不影响视觉效果的情况下减小文件大小。因此此属性的默认值为 true。如果用户需要在工作簿中保留所有样式以用于生成的 html（例如用户稍后需要从生成的 html 恢复工作簿的场景），请将此属性设为 false。 |
| [GetExportDocumentProperties](./getexportdocumentproperties/) | 指示是否导出文档属性。默认值为 true。如果希望将 html 或 mht 文件导入 Excel，请保持默认值。 |
| [SetExportDocumentProperties](./setexportdocumentproperties/) | 指示是否导出文档属性。默认值为 true。如果希望将 html 或 mht 文件导入 Excel，请保持默认值。 |
| [GetExportWorksheetProperties](./getexportworksheetproperties/) | 指示是否导出工作表属性。默认值为 true。如果希望将 html 或 mht 文件导入 Excel，请保持默认值。 |
| [SetExportWorksheetProperties](./setexportworksheetproperties/) | 指示是否导出工作表属性。默认值为 true。如果希望将 html 或 mht 文件导入 Excel，请保持默认值。 |
| [GetExportWorkbookProperties](./getexportworkbookproperties/) | 指示是否导出工作簿属性。默认值为 true。如果希望将 html 或 mht 文件导入 Excel，请保持默认值。 |
| [SetExportWorkbookProperties](./setexportworkbookproperties/) | 指示是否导出工作簿属性。默认值为 true。如果希望将 html 或 mht 文件导入 Excel，请保持默认值。 |
| [GetExportFrameScriptsAndProperties](./getexportframescriptsandproperties/) | 指示是否导出框架脚本和文档属性。默认值为 true。如果希望将 html 或 mht 文件导入 Excel，请保持默认值。 |
| [SetExportFrameScriptsAndProperties](./setexportframescriptsandproperties/) | 指示是否导出框架脚本和文档属性。默认值为 true。如果希望将 html 或 mht 文件导入 Excel，请保持默认值。 |
| [GetExportDataOptions](./getexportdataoptions/) | 指示导出 html 文件数据的规则。默认值为 All。 |
| [SetExportDataOptions](./setexportdataoptions/) | 指示导出 html 文件数据的规则。默认值为 All。 |
| [GetLinkTargetType](./getlinktargettype/) | 指示 <c>&lt;a&gt;</c> 链接中 target 属性的类型。默认值为 HtmlLinkTargetType.Parent。 |
| [SetLinkTargetType](./setlinktargettype/) | 指示 <c>&lt;a&gt;</c> 链接中 target 属性的类型。默认值为 HtmlLinkTargetType.Parent。 |
| [IsIECompatible](./isiecompatible/) | 指示输出的 HTML 是否兼容 IE 浏览器。默认值为 false。 |
| [SetIsIECompatible](./setisiecompatible/) | 指示输出的 HTML 是否兼容 IE 浏览器。默认值为 false。 |
| [GetFormatDataIgnoreColumnWidth](./getformatdataignorecolumnwidth/) | 指示当列溢出时是否显示单元格的完整格式化数据。如果为 true，则忽略列宽，导出单元格的全部数据。如果为 false，则数据的导出方式与 Excel 相同。默认值为 false。 |
| [SetFormatDataIgnoreColumnWidth](./setformatdataignorecolumnwidth/) | 指示当列溢出时是否显示单元格的完整格式化数据。如果为 true，则忽略列宽，导出单元格的全部数据。如果为 false，则数据的导出方式与 Excel 相同。默认值为 false。 |
| [GetCalculateFormula](./getcalculateformula/) | 指示在保存 html 文件之前是否计算公式。 |
| [SetCalculateFormula](./setcalculateformula/) | 指示在保存 html 文件之前是否计算公式。 |
| [IsJsBrowserCompatible](./isjsbrowsercompatible/) | 指示 JavaScript 是否兼容不支持 JavaScript 的浏览器。默认值为 true。 |
| [SetIsJsBrowserCompatible](./setisjsbrowsercompatible/) | 指示 JavaScript 是否兼容不支持 JavaScript 的浏览器。默认值为 true。 |
| [IsMobileCompatible](./ismobilecompatible/) | 指示输出的 HTML 是否兼容移动设备。默认值为 false。 |
| [SetIsMobileCompatible](./setismobilecompatible/) | 指示输出的 HTML 是否兼容移动设备。默认值为 false。 |
| [GetCssStyles](./getcssstyles/) | 获取或设置格式化程序的附加 css 样式。仅在 SaveAsSingleFile 为 True 时有效。 |
| [SetCssStyles](./setcssstyles/) | 获取或设置格式化程序的附加 css 样式。仅在 SaveAsSingleFile 为 True 时有效。 |
| [GetHideOverflowWrappedText](./gethideoverflowwrappedtext/) | 指示当单元格格式设置为自动换行时是否隐藏溢出文本。默认值为 false。 |
| [SetHideOverflowWrappedText](./sethideoverflowwrappedtext/) | 指示当单元格格式设置为自动换行时是否隐藏溢出文本。默认值为 false。 |
| [IsBorderCollapsed](./isbordercollapsed/) | 指示表格边框是否已折叠。默认值为 true。 |
| [SetIsBorderCollapsed](./setisbordercollapsed/) | 指示表格边框是否已折叠。默认值为 true。 |
| [GetEncodeEntityAsCode](./getencodeentityascode/) | 指示是否将 html 字符实体替换为十进制代码。（例如 "&amp;nbsp;" 被替换为 "&amp;#160;"）。默认值为 false。 |
| [SetEncodeEntityAsCode](./setencodeentityascode/) | 指示是否将 html 字符实体替换为十进制代码。（例如 "&amp;nbsp;" 被替换为 "&amp;#160;"）。默认值为 false。 |
| [GetOfficeMathOutputMode](./getofficemathoutputmode/) | 指示 OfficeMath 对象如何导出为 HTML，默认值为 Image。 |
| [SetOfficeMathOutputMode](./setofficemathoutputmode/) | 指示 OfficeMath 对象如何导出为 HTML，默认值为 Image。 |
| [GetCellNameAttribute](./getcellnameattribute/) | 指定指示要写入的 CellName 的属性。（例如，如果值为 "id"，则对于单元格 "A1"，输出将是：&lt;td id='A1'&gt;）。默认值为 null。 |
| [SetCellNameAttribute](./setcellnameattribute/) | 指定指示要写入的 CellName 的属性。（例如，如果值为 "id"，则对于单元格 "A1"，输出将是：&lt;td id='A1'&gt;）。默认值为 null。 |
| [GetDisableCss](./getdisablecss/) | 指示是否仅应用内联样式，而不依赖 CSS。默认值为 false。 |
| [SetDisableCss](./setdisablecss/) | 指示是否仅应用内联样式，而不依赖 CSS。默认值为 false。 |
| [GetEnableCssCustomProperties](./getenablecsscustomproperties/) | 通过使用 CSS 自定义属性优化 html 的输出。例如，在同一 base64 图像出现多次的情况下，使用自定义属性可以只保存一次图像数据，从而提升生成的 html 的性能。默认值为 false。 |
| [SetEnableCssCustomProperties](./setenablecsscustomproperties/) | 通过使用 CSS 自定义属性优化 html 的输出。例如，在同一 base64 图像出现多次的情况下，使用自定义属性可以只保存一次图像数据，从而提升生成的 html 的性能。默认值为 false。 |
| [GetHtmlVersion](./gethtmlversion/) | 指定保存 HTML 格式时应使用的 HTML 标准版本。默认值为 HtmlVersion.Default。 |
| [SetHtmlVersion](./sethtmlversion/) | 指定保存 HTML 格式时应使用的 HTML 标准版本。默认值为 HtmlVersion.Default。 |
| [GetSheetSet](./getsheetset/) | 获取或设置要渲染的工作表。默认是工作簿中所有可见的工作表：Aspose.Cells.Rendering.SheetSet.Visible。 |
| [SetSheetSet](./setsheetset/) | 获取或设置要渲染的工作表。默认是工作簿中所有可见的工作表：Aspose.Cells.Rendering.SheetSet.Visible。 |
| [GetLayoutMode](./getlayoutmode/) | 获取或设置保存为 HTML 时的布局模式。默认值为 HtmlLayoutMode.Normal |
| [SetLayoutMode](./setlayoutmode/) | 获取或设置保存为 HTML 时的布局模式。默认值为 HtmlLayoutMode.Normal |
| [GetEmbeddedFontType](./getembeddedfonttype/) | 获取或设置嵌入到 html 文件中的字体文件类型。默认值为 HtmlEmbeddedFontType.None，表示不会在 html 中嵌入任何字体。 |
| [SetEmbeddedFontType](./setembeddedfonttype/) | 获取或设置嵌入到 html 文件中的字体文件类型。默认值为 HtmlEmbeddedFontType.None，表示不会在 html 中嵌入任何字体。 |
| [GetExportNamedRangeAnchors](./getexportnamedrangeanchors/) | 指示在保存为 HTML 时是否导出命名范围的锚点元素。默认值为 true。 |
| [SetExportNamedRangeAnchors](./setexportnamedrangeanchors/) | 指示在保存为 HTML 时是否导出命名范围的锚点元素。默认值为 true。 |
| [GetDataBarRenderMode](./getdatabarrendermode/) | 表示在将 Excel 文件转换为 html 文件时渲染 DataBar 的模式。默认值为 DataBarRenderMode.BackgroundColor。 |
| [SetDataBarRenderMode](./setdatabarrendermode/) | 表示在将 Excel 文件转换为 html 文件时渲染 DataBar 的模式。默认值为 DataBarRenderMode.BackgroundColor。 |
| [GetSpaceMode](./getspacemode/) | 指示在 HTML 输出中空格的渲染方式。此选项当前仅适用于数字格式（例如会计格式）。默认值为 HtmlSpaceMode.Css。 |
| [SetSpaceMode](./setspacemode/) | 指示在 HTML 输出中空格的渲染方式。此选项当前仅适用于数字格式（例如会计格式）。默认值为 HtmlSpaceMode.Css。 |
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
