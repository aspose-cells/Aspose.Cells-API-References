---
title: "HtmlSaveOptions"
second_title: "Aspose.Cells for Java API 参考"
description: "表示保存 HTML 文件的选项。"
type: docs
url: /zh/java/com.aspose.cells/htmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class HtmlSaveOptions extends SaveOptions
```

表示保存 HTML 文件的选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [HtmlSaveOptions()](#HtmlSaveOptions--) | 创建用于保存 html 文件的选项。 |
| [HtmlSaveOptions(int saveFormat)](#HtmlSaveOptions-int-) | 创建用于保存 htm 文件的选项。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAddGenericFont()](#getAddGenericFont--) | 指示是否向 CSS font-family 添加通用字体。 |
| [getAddTooltipText()](#getAddTooltipText--) | 指示在数据无法完整显示时是否添加工具提示文本。 |
| [getAttachedFilesDirectory()](#getAttachedFilesDirectory--) | 附件文件将保存到的目录。 |
| [getAttachedFilesUrlPrefix()](#getAttachedFilesUrlPrefix--) | 指定 html 文件中附加文件（如图像）的 Url 前缀。 |
| [getCachedFileFolder()](#getCachedFileFolder--) | 用于临时文件的文件夹，可用作数据缓存。 |
| [getCalculateFormula()](#getCalculateFormula--) | 指示是否在保存 html 文件之前计算公式。 |
| [getCellCssPrefix()](#getCellCssPrefix--) | 获取 css 名称的前缀，默认值为 ""。 |
| [getCellNameAttribute()](#getCellNameAttribute--) | 指定指示要写入的 CellName 的属性。 |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | 是否在用户修改单元格相关对象时检查 Excel 文件的限制。 |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | 在保存文件后使工作簿为空。 |
| [getCreateDirectory()](#getCreateDirectory--) | 如果为 true 且目录不存在，目录将在保存文件之前自动创建。 |
| [getCssStyles()](#getCssStyles--) | 获取格式化程序的附加 css 样式。 |
| [getDataBarRenderMode()](#getDataBarRenderMode--) | 表示在将 Excel 文件转换为 html 文件时渲染 DataBar 的模式。 |
| [getDefaultFontName()](#getDefaultFontName--) | 指定导出 html 时的默认字体名称，当样式的字体不存在时将使用默认字体；如果此属性为 null，Aspose.Cells 将使用与原始字体同一系列的通用字体，默认值为 null。 |
| [getDisableCss()](#getDisableCss--) | 指示是否仅应用内联样式，而不依赖 CSS。 |
| [getDisableDownlevelRevealedComments()](#getDisableDownlevelRevealedComments--) | 指示在导出文件为 html 时是否禁用 Downlevel-revealed 条件注释，默认值为 false。 |
| [getEmbeddedFontType()](#getEmbeddedFontType--) | 获取嵌入字体文件到 html 文件的类型。 |
| [getEnableCssCustomProperties()](#getEnableCssCustomProperties--) | 通过使用 CSS 自定义属性来优化 html 的输出。 |
| [getEncodeEntityAsCode()](#getEncodeEntityAsCode--) | 指示是否将 html 字符实体替换为十进制代码。 |
| [getEncoding()](#getEncoding--) | 如果未设置，则使用 Encoding.UTF8 作为默认编码类型。 |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | 指示在保存为 .xls 文件时是否加密文档属性。 |
| [getExcludeUnusedStyles()](#getExcludeUnusedStyles--) | 指示是否排除未使用的样式。 |
| [getExportActiveWorksheetOnly()](#getExportActiveWorksheetOnly--) | 指示是否仅将活动工作表导出为 html 文件。 |
| [getExportArea()](#getExportArea--) | 获取当前活动工作表的导出 CellArea。 |
| [getExportBogusRowData()](#getExportBogusRowData--) | 指示是否导出虚假的底部行数据。 |
| [getExportCellCoordinate()](#getExportCellCoordinate--) | 指示在将文件保存为 html 时是否导出非空单元格的 Excel 坐标。 |
| [getExportCommentsType()](#getExportCommentsType--) | 表示导出注释到 html 文件的类型。 |
| [getExportDataOptions()](#getExportDataOptions--) | 指示导出 html 文件数据的规则。默认值为 All。 |
| [getExportDocumentProperties()](#getExportDocumentProperties--) | 指示是否导出文档属性。默认值为 true。如果要将 html 或 mht 文件导入到 excel，请保持默认值。 |
| [getExportExtraHeadings()](#getExportExtraHeadings--) | 指示当文本长度超过最大显示列时是否导出额外的标题。 |
| [getExportFormula()](#getExportFormula--) | 指示在将文件保存为 html 时是否导出公式。 |
| [getExportFrameScriptsAndProperties()](#getExportFrameScriptsAndProperties--) | 指示是否导出框架脚本和文档属性。 |
| [getExportGridLines()](#getExportGridLines--) | 指示是否导出网格线。默认值为 false。 |
| [getExportHeadings()](#getExportHeadings--) | 指示在保存为 HTML 文件时是否导出工作表的行列标题。 |
| [getExportHiddenWorksheet()](#getExportHiddenWorksheet--) | 指示是否导出隐藏工作表的内容。默认值为 true。 |
| [getExportImagesAsBase64()](#getExportImagesAsBase64--) | 指定图像是否以 Base64 格式保存到 HTML、MHTML 或 EPUB。 |
| [getExportNamedRangeAnchors()](#getExportNamedRangeAnchors--) | 指示在保存为 HTML 时是否导出命名范围的锚点元素。 |
| [getExportObjectListener()](#getExportObjectListener--) | 获取用于导出对象的 ExportObjectListener。 |
| [getExportPageFooters()](#getExportPageFooters--) | 指示是否导出页面标题。 |
| [getExportPageHeaders()](#getExportPageHeaders--) | 指示是否导出页面标题。 |
| [getExportPrintAreaOnly()](#getExportPrintAreaOnly--) | 指示是否仅将打印区域导出为 HTML 文件。 |
| [getExportRowColumnHeadings()](#getExportRowColumnHeadings--) | 指示在保存为 HTML 文件时是否导出工作表的行列标题。 |
| [getExportSimilarBorderStyle()](#getExportSimilarBorderStyle--) | 指示在浏览器不支持的情况下是否导出相似的边框样式。 |
| [getExportSingleTab()](#getExportSingleTab--) | 指示当文件只有一个工作表时是否导出单个标签页。 |
| [getExportWorkbookProperties()](#getExportWorkbookProperties--) | 指示是否导出工作簿属性。默认值为 true。如果您想将 html 或 mht 文件导入 Excel，请保持默认值。 |
| [getExportWorksheetCSSSeparately()](#getExportWorksheetCSSSeparately--) | 指示是否单独导出工作表 CSS。默认值为 false。 |
| [getExportWorksheetProperties()](#getExportWorksheetProperties--) | 指示是否导出工作表属性。默认值为 true。如果您想将 html 或 mht 文件导入 Excel，请保持默认值。 |
| [getFilePathProvider()](#getFilePathProvider--) | 获取用于单独将工作表导出为 HTML 的 IFilePathProvider。 |
| [getFormatDataIgnoreColumnWidth()](#getFormatDataIgnoreColumnWidth--) | 指示当列溢出时是否显示单元格的完整格式化数据。 |
| [getHiddenColDisplayType()](#getHiddenColDisplayType--) | 在 Excel 中隐藏列（此列宽度为 0），在保存为 HTML 格式之前，如果 HtmlHiddenColDisplayType 为 \"Remove\"，则隐藏列不会被输出；如果该值为 \"Hidden\"，列会被输出，但仍保持隐藏，默认值为 \"Hidden\"。 |
| [getHiddenRowDisplayType()](#getHiddenRowDisplayType--) | 在 Excel 中隐藏行（此行高度为 0），在保存为 HTML 格式之前，如果 HtmlHiddenRowDisplayType 为 \"Remove\"，则隐藏行不会被输出；如果该值为 \"Hidden\"，行会被输出，但仍保持隐藏，默认值为 \"Hidden\"。 |
| [getHideOverflowWrappedText()](#getHideOverflowWrappedText--) | 指示当单元格格式设置为自动换行时是否隐藏溢出文本。 |
| [getHtmlCrossStringType()](#getHtmlCrossStringType--) | 指示在将 Excel 文件保存为 HTML 格式时，跨单元格字符串是否以与 MS Excel 相同的方式显示。 |
| [getHtmlVersion()](#getHtmlVersion--) | 指定保存为 HTML 格式时应使用的 HTML 标准版本。 |
| [getIgnoreInvisibleShapes()](#getIgnoreInvisibleShapes--) | 指示是否导出不可见的形状。 |
| [getImageOptions()](#getImageOptions--) | 在导出之前获取 ImageOrPrintOptions 对象。 |
| [getImageScalable()](#getImageScalable--) | 指示在使用可伸缩单位描述列宽时，是否使用可伸缩单位描述图像宽度。 |
| [getLayoutMode()](#getLayoutMode--) | 获取保存为 HTML 时的布局模式。 |
| [getLinkTargetType()](#getLinkTargetType--) | 指示 `<a>` 链接中 target 属性的类型。 |
| [getMergeAreas()](#getMergeAreas--) | 指示在保存文件之前是否合并条件格式和验证的区域。 |
| [getMergeEmptyTdForcely()](#getMergeEmptyTdForcely--) | 指示在导出文件为 HTML 时是否强制合并空的 TD 元素。 |
| [getMergeEmptyTdType()](#getMergeEmptyTdType--) | 合并连续空单元格（空 td 元素）的选项。默认值为 MergeEmptyTdType.Default。 |
| [getOfficeMathOutputMode()](#getOfficeMathOutputMode--) | 指示 OfficeMath 对象如何导出为 HTML，默认值为 Image。 |
| [getPageTitle()](#getPageTitle--) | HTML 页面标题。 |
| [getParseHtmlTagInCell()](#getParseHtmlTagInCell--) | 指示单元格中的 HTML 标签（例如 `<div></div>`）是应解析为单元格值还是保持原样。 |
| [getPresentationPreference()](#getPresentationPreference--) | 指示 html 或 mht 文件是否为演示首选。 |
| [getRefreshChartCache()](#getRefreshChartCache--) | 指示是否缓存图表的最新数据。 |
| [getSaveAsSingleFile()](#getSaveAsSingleFile--) | 指示是否将 HTML 保存为单个文件。 |
| [getSaveFormat()](#getSaveFormat--) | 获取保存的文件格式。 |
| [getSheetSet()](#getSheetSet--) | 获取要渲染的工作表。 |
| [getShowAllSheets()](#getShowAllSheets--) | 指示在保存为单个 HTML 文件时是否显示所有工作表。 |
| [getSortExternalNames()](#getSortExternalNames--) | 指示在保存文件之前是否对外部已定义名称进行排序。 |
| [getSortNames()](#getSortNames--) | 指示在保存文件之前是否对已定义名称进行排序。 |
| [getSpaceMode()](#getSpaceMode--) | 指示空格在 HTML 输出中的渲染方式。 |
| [getStreamProvider()](#getStreamProvider--) | 获取用于导出对象的 IStreamProvider。 |
| [getTableCssId()](#getTableCssId--) | 获取类型 CSS 名称的前缀，如 tr、col、td 等，它们包含在具有特定 TableCssId 属性的 table 元素中。 |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | 指示是否更新 SmartArt 设置。 |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | 指示在保存文件之前是否验证合并的单元格。 |
| [getWarningCallback()](#getWarningCallback--) | 获取警告回调。 |
| [getWidthScalable()](#getWidthScalable--) | 指示是否以比例单位将列宽导出到 HTML。 |
| [getWorksheetScalable()](#getWorksheetScalable--) | 指示在将文件保存为 HTML 时是否通过工作表缩放级别对 HTML 进行放大或缩小，默认值为 false。 |
| [hashCode()](#hashCode--) |  |
| [isBorderCollapsed()](#isBorderCollapsed--) | 指示表格边框是否已折叠。 |
| [isExpImageToTempDir()](#isExpImageToTempDir--) | 指示是否将图像文件导出到临时目录。 |
| [isExportComments()](#isExportComments--) | 指示在将文件保存为 HTML 时是否导出注释，默认值为 false。 |
| [isFullPathLink()](#isFullPathLink--) | 指示在 sheet00x.htm、filelist.xml 和 tabstrip.htm 中是否使用完整路径链接。 |
| [isIECompatible()](#isIECompatible--) | 指示输出的 HTML 是否兼容 IE 浏览器。 |
| [isJsBrowserCompatible()](#isJsBrowserCompatible--) | 指示 JavaScript 是否兼容不支持 JavaScript 的浏览器。 |
| [isMobileCompatible()](#isMobileCompatible--) | 指示输出的 HTML 是否兼容移动设备。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAddGenericFont(boolean value)](#setAddGenericFont-boolean-) | 指示是否向 CSS font-family 添加通用字体。 |
| [setAddTooltipText(boolean value)](#setAddTooltipText-boolean-) | 指示在数据无法完整显示时是否添加工具提示文本。 |
| [setAttachedFilesDirectory(String value)](#setAttachedFilesDirectory-java.lang.String-) | 附件文件将保存到的目录。 |
| [setAttachedFilesUrlPrefix(String value)](#setAttachedFilesUrlPrefix-java.lang.String-) | 指定 html 文件中附加文件（如图像）的 Url 前缀。 |
| [setBorderCollapsed(boolean value)](#setBorderCollapsed-boolean-) | 指示表格边框是否已折叠。 |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | 用于临时文件的文件夹，可用作数据缓存。 |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | 指示是否在保存 html 文件之前计算公式。 |
| [setCellCssPrefix(String value)](#setCellCssPrefix-java.lang.String-) | 设置 CSS 名称的前缀，默认值为 ""。 |
| [setCellNameAttribute(String value)](#setCellNameAttribute-java.lang.String-) | 指定指示要写入的 CellName 的属性。 |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | 是否在用户修改单元格相关对象时检查 Excel 文件的限制。 |
| [setClearData(boolean value)](#setClearData-boolean-) | 在保存文件后使工作簿为空。 |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | 如果为 true 且目录不存在，目录将在保存文件之前自动创建。 |
| [setCssStyles(String value)](#setCssStyles-java.lang.String-) | 设置格式化程序的附加 CSS 样式。 |
| [setDataBarRenderMode(int value)](#setDataBarRenderMode-int-) | 表示在将 Excel 文件转换为 html 文件时渲染 DataBar 的模式。 |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | 指定导出 html 时的默认字体名称，当样式的字体不存在时将使用默认字体；如果此属性为 null，Aspose.Cells 将使用与原始字体同一系列的通用字体，默认值为 null。 |
| [setDisableCss(boolean value)](#setDisableCss-boolean-) | 指示是否仅应用内联样式，而不依赖 CSS。 |
| [setDisableDownlevelRevealedComments(boolean value)](#setDisableDownlevelRevealedComments-boolean-) | 指示在导出文件为 html 时是否禁用 Downlevel-revealed 条件注释，默认值为 false。 |
| [setEmbeddedFontType(int value)](#setEmbeddedFontType-int-) | 设置将字体文件嵌入 HTML 文件的类型。 |
| [setEnableCssCustomProperties(boolean value)](#setEnableCssCustomProperties-boolean-) | 通过使用 CSS 自定义属性来优化 html 的输出。 |
| [setEncodeEntityAsCode(boolean value)](#setEncodeEntityAsCode-boolean-) | 指示是否将 html 字符实体替换为十进制代码。 |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | 如果未设置，则使用 Encoding.UTF8 作为默认编码类型。 |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | 指示在保存为 .xls 文件时是否加密文档属性。 |
| [setExcludeUnusedStyles(boolean value)](#setExcludeUnusedStyles-boolean-) | 指示是否排除未使用的样式。 |
| [setExpImageToTempDir(boolean value)](#setExpImageToTempDir-boolean-) | 指示是否将图像文件导出到临时目录。 |
| [setExportActiveWorksheetOnly(boolean value)](#setExportActiveWorksheetOnly-boolean-) | 指示是否仅将活动工作表导出为 html 文件。 |
| [setExportArea(CellArea value)](#setExportArea-com.aspose.cells.CellArea-) | 设置当前活动工作表的导出 CellArea。 |
| [setExportBogusRowData(boolean value)](#setExportBogusRowData-boolean-) | 指示是否导出虚假的底部行数据。 |
| [setExportCellCoordinate(boolean value)](#setExportCellCoordinate-boolean-) | 指示在将文件保存为 html 时是否导出非空单元格的 Excel 坐标。 |
| [setExportComments(boolean value)](#setExportComments-boolean-) | 指示在将文件保存为 HTML 时是否导出注释，默认值为 false。 |
| [setExportCommentsType(int value)](#setExportCommentsType-int-) | 表示导出注释到 html 文件的类型。 |
| [setExportDataOptions(int value)](#setExportDataOptions-int-) | 指示导出 html 文件数据的规则。默认值为 All。 |
| [setExportDocumentProperties(boolean value)](#setExportDocumentProperties-boolean-) | 指示是否导出文档属性。默认值为 true。如果要将 html 或 mht 文件导入到 excel，请保持默认值。 |
| [setExportExtraHeadings(boolean value)](#setExportExtraHeadings-boolean-) | 指示当文本长度超过最大显示列时是否导出额外的标题。 |
| [setExportFormula(boolean value)](#setExportFormula-boolean-) | 指示在将文件保存为 html 时是否导出公式。 |
| [setExportFrameScriptsAndProperties(boolean value)](#setExportFrameScriptsAndProperties-boolean-) | 指示是否导出框架脚本和文档属性。 |
| [setExportGridLines(boolean value)](#setExportGridLines-boolean-) | 指示是否导出网格线。默认值为 false。 |
| [setExportHeadings(boolean value)](#setExportHeadings-boolean-) | 指示在保存为 HTML 文件时是否导出工作表的行列标题。 |
| [setExportHiddenWorksheet(boolean value)](#setExportHiddenWorksheet-boolean-) | 指示是否导出隐藏工作表的内容。默认值为 true。 |
| [setExportImagesAsBase64(boolean value)](#setExportImagesAsBase64-boolean-) | 指定图像是否以 Base64 格式保存到 HTML、MHTML 或 EPUB。 |
| [setExportNamedRangeAnchors(boolean value)](#setExportNamedRangeAnchors-boolean-) | 指示在保存为 HTML 时是否导出命名范围的锚点元素。 |
| [setExportObjectListener(IExportObjectListener value)](#setExportObjectListener-com.aspose.cells.IExportObjectListener-) | 设置用于导出对象的 ExportObjectListener。 |
| [setExportPageFooters(boolean value)](#setExportPageFooters-boolean-) | 指示是否导出页面标题。 |
| [setExportPageHeaders(boolean value)](#setExportPageHeaders-boolean-) | 指示是否导出页面标题。 |
| [setExportPrintAreaOnly(boolean value)](#setExportPrintAreaOnly-boolean-) | 指示是否仅将打印区域导出为 HTML 文件。 |
| [setExportRowColumnHeadings(boolean value)](#setExportRowColumnHeadings-boolean-) | 指示在保存为 HTML 文件时是否导出工作表的行列标题。 |
| [setExportSimilarBorderStyle(boolean value)](#setExportSimilarBorderStyle-boolean-) | 指示在浏览器不支持的情况下是否导出相似的边框样式。 |
| [setExportSingleTab(boolean value)](#setExportSingleTab-boolean-) | 指示当文件只有一个工作表时是否导出单个标签页。 |
| [setExportWorkbookProperties(boolean value)](#setExportWorkbookProperties-boolean-) | 指示是否导出工作簿属性。默认值为 true。如果您想将 html 或 mht 文件导入 Excel，请保持默认值。 |
| [setExportWorksheetCSSSeparately(boolean value)](#setExportWorksheetCSSSeparately-boolean-) | 指示是否单独导出工作表 CSS。默认值为 false。 |
| [setExportWorksheetProperties(boolean value)](#setExportWorksheetProperties-boolean-) | 指示是否导出工作表属性。默认值为 true。如果您想将 html 或 mht 文件导入 Excel，请保持默认值。 |
| [setFilePathProvider(IFilePathProvider value)](#setFilePathProvider-com.aspose.cells.IFilePathProvider-) | 设置用于单独导出工作表到 HTML 的 IFilePathProvider。 |
| [setFormatDataIgnoreColumnWidth(boolean value)](#setFormatDataIgnoreColumnWidth-boolean-) | 指示当列溢出时是否显示单元格的完整格式化数据。 |
| [setFullPathLink(boolean value)](#setFullPathLink-boolean-) | 指示在 sheet00x.htm、filelist.xml 和 tabstrip.htm 中是否使用完整路径链接。 |
| [setHiddenColDisplayType(int value)](#setHiddenColDisplayType-int-) | 在 Excel 中隐藏列（此列宽度为 0），在保存为 HTML 格式之前，如果 HtmlHiddenColDisplayType 为 \"Remove\"，则隐藏列不会被输出；如果该值为 \"Hidden\"，列会被输出，但仍保持隐藏，默认值为 \"Hidden\"。 |
| [setHiddenRowDisplayType(int value)](#setHiddenRowDisplayType-int-) | 在 Excel 中隐藏行（此行高度为 0），在保存为 HTML 格式之前，如果 HtmlHiddenRowDisplayType 为 \"Remove\"，则隐藏行不会被输出；如果该值为 \"Hidden\"，行会被输出，但仍保持隐藏，默认值为 \"Hidden\"。 |
| [setHideOverflowWrappedText(boolean value)](#setHideOverflowWrappedText-boolean-) | 指示当单元格格式设置为自动换行时是否隐藏溢出文本。 |
| [setHtmlCrossStringType(int value)](#setHtmlCrossStringType-int-) | 指示在将 Excel 文件保存为 HTML 格式时，跨单元格字符串是否以与 MS Excel 相同的方式显示。 |
| [setHtmlVersion(int value)](#setHtmlVersion-int-) | 指定保存为 HTML 格式时应使用的 HTML 标准版本。 |
| [setIECompatible(boolean value)](#setIECompatible-boolean-) | 指示输出的 HTML 是否兼容 IE 浏览器。 |
| [setIgnoreInvisibleShapes(boolean value)](#setIgnoreInvisibleShapes-boolean-) | 指示是否导出不可见的形状。 |
| [setImageScalable(boolean value)](#setImageScalable-boolean-) | 指示在使用可伸缩单位描述列宽时，是否使用可伸缩单位描述图像宽度。 |
| [setJsBrowserCompatible(boolean value)](#setJsBrowserCompatible-boolean-) | 指示 JavaScript 是否兼容不支持 JavaScript 的浏览器。 |
| [setLayoutMode(int value)](#setLayoutMode-int-) | 设置保存为 HTML 时的布局模式。 |
| [setLinkTargetType(int value)](#setLinkTargetType-int-) | 指示 `<a>` 链接中 target 属性的类型。 |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | 指示在保存文件之前是否合并条件格式和验证的区域。 |
| [setMergeEmptyTdForcely(boolean value)](#setMergeEmptyTdForcely-boolean-) | 指示在导出文件为 HTML 时是否强制合并空的 TD 元素。 |
| [setMergeEmptyTdType(int value)](#setMergeEmptyTdType-int-) | 合并连续空单元格（空 td 元素）的选项。默认值为 MergeEmptyTdType.Default。 |
| [setMobileCompatible(boolean value)](#setMobileCompatible-boolean-) | 指示输出的 HTML 是否兼容移动设备。 |
| [setOfficeMathOutputMode(int value)](#setOfficeMathOutputMode-int-) | 指示 OfficeMath 对象如何导出为 HTML，默认值为 Image。 |
| [setPageTitle(String value)](#setPageTitle-java.lang.String-) | HTML 页面标题。 |
| [setParseHtmlTagInCell(boolean value)](#setParseHtmlTagInCell-boolean-) | 指示单元格中的 HTML 标签（例如 `<div></div>`）是应解析为单元格值还是保持原样。 |
| [setPresentationPreference(boolean value)](#setPresentationPreference-boolean-) | 指示 html 或 mht 文件是否为演示首选。 |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | 指示是否缓存图表的最新数据。 |
| [setSaveAsSingleFile(boolean value)](#setSaveAsSingleFile-boolean-) | 指示是否将 HTML 保存为单个文件。 |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | 设置要渲染的工作表。 |
| [setShowAllSheets(boolean value)](#setShowAllSheets-boolean-) | 指示在保存为单个 HTML 文件时是否显示所有工作表。 |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | 指示在保存文件之前是否对外部已定义名称进行排序。 |
| [setSortNames(boolean value)](#setSortNames-boolean-) | 指示在保存文件之前是否对已定义名称进行排序。 |
| [setSpaceMode(int value)](#setSpaceMode-int-) | 指示空格在 HTML 输出中的渲染方式。 |
| [setStreamProvider(IStreamProvider value)](#setStreamProvider-com.aspose.cells.IStreamProvider-) | 设置用于导出对象的 IStreamProvider。 |
| [setTableCssId(String value)](#setTableCssId-java.lang.String-) | 设置类型 CSS 名称的前缀，如 tr、col、td 等，它们包含在具有特定 TableCssId 属性的 table 元素中。 |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | 指示是否更新 SmartArt 设置。 |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | 指示在保存文件之前是否验证合并的单元格。 |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | 设置警告回调。 |
| [setWidthScalable(boolean value)](#setWidthScalable-boolean-) | 指示是否以比例单位将列宽导出到 HTML。 |
| [setWorksheetScalable(boolean value)](#setWorksheetScalable-boolean-) | 指示在将文件保存为 HTML 时是否通过工作表缩放级别对 HTML 进行放大或缩小，默认值为 false。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### HtmlSaveOptions() {#HtmlSaveOptions--}
```
public HtmlSaveOptions()
```


创建用于保存 html 文件的选项。

### HtmlSaveOptions(int saveFormat) {#HtmlSaveOptions-int-}
```
public HtmlSaveOptions(int saveFormat)
```


创建用于保存 htm 文件的选项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat)。文件格式。它应该是以下类型之一：[SaveFormat.HTML](../../com.aspose.cells/saveformat\#HTML) 或 [SaveFormat.M\_HTML](../../com.aspose.cells/saveformat\#M-HTML)，否则保存的格式将自动设置为 [SaveFormat.HTML](../../com.aspose.cells/saveformat\#HTML)。 |

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
### getAddGenericFont() {#getAddGenericFont--}
```
public boolean getAddGenericFont()
```


指示是否向 CSS font-family 添加通用字体。默认值为 true。

**Returns:**
boolean
### getAddTooltipText() {#getAddTooltipText--}
```
public boolean getAddTooltipText()
```


指示在数据无法完整显示时是否添加工具提示文本。默认值为 false。

**Returns:**
boolean
### getAttachedFilesDirectory() {#getAttachedFilesDirectory--}
```
public String getAttachedFilesDirectory()
```


附加文件将保存到的目录。仅用于保存为 html 流。

**Returns:**
java.lang.String
### getAttachedFilesUrlPrefix() {#getAttachedFilesUrlPrefix--}
```
public String getAttachedFilesUrlPrefix()
```


指定附加文件（如 html 文件中的图像）的 Url 前缀。仅用于保存为 html 流。

**Returns:**
java.lang.String
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


用于临时文件的文件夹，可用作数据缓存。

**Remarks**

如果未指定文件夹，则其默认值为 [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--)。如果其默认值为 null 或为空，或已指定为 null 或为空，则在保存工作簿时不会使用缓存文件。

**Returns:**
java.lang.String
### getCalculateFormula() {#getCalculateFormula--}
```
public boolean getCalculateFormula()
```


指示是否在保存 html 文件之前计算公式。

**Remarks**

默认值为 false。

**Returns:**
boolean
### getCellCssPrefix() {#getCellCssPrefix--}
```
public String getCellCssPrefix()
```


获取 css 名称的前缀，默认值为 ""。

**Returns:**
java.lang.String
### getCellNameAttribute() {#getCellNameAttribute--}
```
public String getCellNameAttribute()
```


指定用于写入 CellName 的属性。（例如，如果值为 "id"，则单元格 "A1" 的输出将是：<td id='A1'>）。默认值为 null。

**Returns:**
java.lang.String
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


是否在用户修改单元格相关对象时检查 Excel 文件的限制。例如，Excel 不允许输入超过 32K 的字符串值。当您输入超过 32K 的值时，它将被截断。

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getClearData() {#getClearData--}
```
public boolean getClearData()
```


在保存文件后使工作簿为空。

**Returns:**
boolean
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


如果为 true 且目录不存在，目录将在保存文件之前自动创建。

**Remarks**

默认值为 false。

**Returns:**
boolean
### getCssStyles() {#getCssStyles--}
```
public String getCssStyles()
```


获取格式化程序的附加 css 样式。仅在 [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) 为 True 时有效。CssStyles="body \{ padding: 5px \}";

**Returns:**
java.lang.String
### getDataBarRenderMode() {#getDataBarRenderMode--}
```
public int getDataBarRenderMode()
```


表示在将 Excel 文件转换为 html 文件时渲染 DataBar 的模式。默认值为 [DataBarRenderMode.BACKGROUND\_COLOR](../../com.aspose.cells/databarrendermode\#BACKGROUND-COLOR)。

参见 [DataBarRenderMode](../../com.aspose.cells/databarrendermode)。

**Returns:**
int
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```


指定导出 html 时的默认字体名称，当样式的字体不存在时将使用默认字体；如果此属性为 null，Aspose.Cells 将使用与原始字体同一系列的通用字体，默认值为 null。

**Returns:**
java.lang.String
### getDisableCss() {#getDisableCss--}
```
public boolean getDisableCss()
```


指示是否仅应用内联样式，而不依赖 CSS。默认值为 false。

**Returns:**
boolean
### getDisableDownlevelRevealedComments() {#getDisableDownlevelRevealedComments--}
```
public boolean getDisableDownlevelRevealedComments()
```


指示在导出文件为 html 时是否禁用 Downlevel-revealed 条件注释，默认值为 false。

**Returns:**
boolean
### getEmbeddedFontType() {#getEmbeddedFontType--}
```
public int getEmbeddedFontType()
```


获取嵌入字体文件到 html 文件的类型。默认值为 [HtmlEmbeddedFontType.NONE](../../com.aspose.cells/htmlembeddedfonttype\#NONE)，表示不会在 html 中嵌入任何字体。

参见 [HtmlEmbeddedFontType](../../com.aspose.cells/htmlembeddedfonttype)。

**Returns:**
int
### getEnableCssCustomProperties() {#getEnableCssCustomProperties--}
```
public boolean getEnableCssCustomProperties()
```


通过使用 CSS 自定义属性优化 html 的输出。例如，在同一 base64 图像出现多次的情况下，使用自定义属性只需保存一次图像数据，从而提升生成的 html 性能。默认值为 false。

**Returns:**
boolean
### getEncodeEntityAsCode() {#getEncodeEntityAsCode--}
```
public boolean getEncodeEntityAsCode()
```


指示是否将 html 字符实体替换为十进制代码。（例如，"&nbsp;" 被替换为 "&\#160;"）。默认值为 false。

**Returns:**
boolean
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


如果未设置，则使用 Encoding.UTF8 作为默认编码类型。

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```
public boolean getEncryptDocumentProperties()
```


指示在保存为 .xls 文件时是否加密文档属性。默认值为 true。

**Remarks**

仅适用于 .xls、xlsx、xlsb 和 xlsm 文件。

**Returns:**
boolean
### getExcludeUnusedStyles() {#getExcludeUnusedStyles--}
```
public boolean getExcludeUnusedStyles()
```


指示是否排除未使用的样式。对于生成的 html 文件，排除未使用的样式可以在不影响视觉效果的前提下降小文件大小。因此此属性的默认值为 true。如果用户需要在工作簿中保留所有样式以供生成的 html 使用（例如用户稍后需要从生成的 html 恢复工作簿），请将此属性设为 false。

**Returns:**
boolean
### getExportActiveWorksheetOnly() {#getExportActiveWorksheetOnly--}
```
public boolean getExportActiveWorksheetOnly()
```


指示是否仅导出活动工作表到 html 文件。如果为 true，则仅导出活动工作表；如果为 false，则导出整个工作簿。默认值为 false。

**Returns:**
boolean
### getExportArea() {#getExportArea--}
```
public CellArea getExportArea()
```


获取当前活动工作表的导出 CellArea。如果设置此属性，当前活动工作表的打印区域将被省略。保存为 html 时仅导出指定的区域。

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getExportBogusRowData() {#getExportBogusRowData--}
```
public boolean getExportBogusRowData()
```


指示是否导出虚假的底部行数据。默认值为 true。如果希望将 html 或 mht 文件导入 Excel，请保持默认值。

**Returns:**
boolean
### getExportCellCoordinate() {#getExportCellCoordinate--}
```
public boolean getExportCellCoordinate()
```


指示在保存文件为 html 时是否导出非空单元格的 Excel 坐标。默认值为 false。如果希望将生成的 html 导入 Excel，请保持默认值。

**Returns:**
boolean
### getExportCommentsType() {#getExportCommentsType--}
```
public int getExportCommentsType()
```


表示导出注释到 html 文件的类型。

参见 [PrintCommentsType](../../com.aspose.cells/printcommentstype)。

**Returns:**
int
### getExportDataOptions() {#getExportDataOptions--}
```
public int getExportDataOptions()
```


指示导出 html 文件数据的规则。默认值为 All。

参见 [HtmlExportDataOptions](../../com.aspose.cells/htmlexportdataoptions)。

**Returns:**
int
### getExportDocumentProperties() {#getExportDocumentProperties--}
```
public boolean getExportDocumentProperties()
```


指示是否导出文档属性。默认值为 true。如果要将 html 或 mht 文件导入到 excel，请保持默认值。

**Returns:**
boolean
### getExportExtraHeadings() {#getExportExtraHeadings--}
```
public boolean getExportExtraHeadings()
```


指示当文本长度超过最大显示列时是否导出额外的标题。默认值为 false。如果希望将 html 文件导入 Excel，请保持默认值。

**Returns:**
boolean
### getExportFormula() {#getExportFormula--}
```
public boolean getExportFormula()
```


指示在保存文件为 html 时是否导出公式。默认值为 true。如果希望将生成的 html 导入 Excel，请保持默认值。

**Returns:**
boolean
### getExportFrameScriptsAndProperties() {#getExportFrameScriptsAndProperties--}
```
public boolean getExportFrameScriptsAndProperties()
```


指示是否导出框架脚本和文档属性。默认值为 true。如果希望将 html 或 mht 文件导入 Excel，请保持默认值。

**Returns:**
boolean
### getExportGridLines() {#getExportGridLines--}
```
public boolean getExportGridLines()
```


指示是否导出网格线。默认值为 false。

**Returns:**
boolean
### getExportHeadings() {#getExportHeadings--}
```
public boolean getExportHeadings()
```


指示在保存为 HTML 文件时是否导出工作表的行列标题。

**Remarks**

注意：此成员现已过时。请改用 HtmlSaveOptions.ExportRowColumnHeadings 属性。此属性将在自 2022 年 6 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
boolean
### getExportHiddenWorksheet() {#getExportHiddenWorksheet--}
```
public boolean getExportHiddenWorksheet()
```


指示是否导出隐藏工作表的内容。默认值为 true。

**Returns:**
boolean
### getExportImagesAsBase64() {#getExportImagesAsBase64--}
```
public boolean getExportImagesAsBase64()
```


指定图像是否以 Base64 格式保存到 HTML、MHTML 或 EPUB。

**Remarks**

当此属性设置为 true 时，图像数据直接导出到 img 元素上，不会创建单独的文件。

**Returns:**
boolean
### getExportNamedRangeAnchors() {#getExportNamedRangeAnchors--}
```
public boolean getExportNamedRangeAnchors()
```


指示在保存为 HTML 时是否导出命名范围的锚点元素。默认值为 true。

**Returns:**
boolean
### getExportObjectListener() {#getExportObjectListener--}
```
public IExportObjectListener getExportObjectListener()
```


获取用于导出对象的 ExportObjectListener。

**Remarks**

注意：此属性已过时。请改用 HtmlSaveOptions.IStreamProvider 属性。该属性将在自 2015 年 8 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
[IExportObjectListener](../../com.aspose.cells/iexportobjectlistener)
### getExportPageFooters() {#getExportPageFooters--}
```
public boolean getExportPageFooters()
```


指示是否导出页面标题。

**Remarks**

仅在 [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) 为 True 时有效。

**Returns:**
boolean
### getExportPageHeaders() {#getExportPageHeaders--}
```
public boolean getExportPageHeaders()
```


指示是否导出页面标题。

**Remarks**

仅在 [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) 为 True 时有效。

**Returns:**
boolean
### getExportPrintAreaOnly() {#getExportPrintAreaOnly--}
```
public boolean getExportPrintAreaOnly()
```


指示是否仅导出打印区域到 HTML 文件。默认值为 false。

**Returns:**
boolean
### getExportRowColumnHeadings() {#getExportRowColumnHeadings--}
```
public boolean getExportRowColumnHeadings()
```


指示在保存为 HTML 文件时是否导出工作表的行列标题。

**Remarks**

默认值为 false。

**Returns:**
boolean
### getExportSimilarBorderStyle() {#getExportSimilarBorderStyle--}
```
public boolean getExportSimilarBorderStyle()
```


指示在浏览器不支持的情况下是否导出相似的边框样式。如果您想将 html 或 mht 文件导入到 Excel，请保持默认值。默认值为 false。

**Returns:**
boolean
### getExportSingleTab() {#getExportSingleTab--}
```
public boolean getExportSingleTab()
```


指示当文件仅包含一个工作表时是否导出单个标签页。默认值为 false。

**Returns:**
boolean
### getExportWorkbookProperties() {#getExportWorkbookProperties--}
```
public boolean getExportWorkbookProperties()
```


指示是否导出工作簿属性。默认值为 true。如果您想将 html 或 mht 文件导入 Excel，请保持默认值。

**Returns:**
boolean
### getExportWorksheetCSSSeparately() {#getExportWorksheetCSSSeparately--}
```
public boolean getExportWorksheetCSSSeparately()
```


指示是否单独导出工作表 CSS。默认值为 false。

**Returns:**
boolean
### getExportWorksheetProperties() {#getExportWorksheetProperties--}
```
public boolean getExportWorksheetProperties()
```


指示是否导出工作表属性。默认值为 true。如果您想将 html 或 mht 文件导入 Excel，请保持默认值。

**Returns:**
boolean
### getFilePathProvider() {#getFilePathProvider--}
```
public IFilePathProvider getFilePathProvider()
```


获取用于单独将工作表导出为 HTML 的 IFilePathProvider。

**Returns:**
[IFilePathProvider](../../com.aspose.cells/ifilepathprovider)
### getFormatDataIgnoreColumnWidth() {#getFormatDataIgnoreColumnWidth--}
```
public boolean getFormatDataIgnoreColumnWidth()
```


指示当内容溢出列时是否显示单元格的完整格式化数据。如果为 true，则忽略列宽并导出单元格的全部数据；如果为 false，则数据的导出方式与 Excel 相同。默认值为 false。

**Returns:**
boolean
### getHiddenColDisplayType() {#getHiddenColDisplayType--}
```
public int getHiddenColDisplayType()
```


在 Excel 中隐藏列（此列宽度为 0），在保存为 HTML 格式之前，如果 HtmlHiddenColDisplayType 为 \"Remove\"，则隐藏列不会被输出；如果该值为 \"Hidden\"，列会被输出，但仍保持隐藏，默认值为 \"Hidden\"。

参见 [HtmlHiddenColDisplayType](../../com.aspose.cells/htmlhiddencoldisplaytype)。

**Returns:**
int
### getHiddenRowDisplayType() {#getHiddenRowDisplayType--}
```
public int getHiddenRowDisplayType()
```


在 Excel 中隐藏行（此行高度为 0），在保存为 HTML 格式之前，如果 HtmlHiddenRowDisplayType 为 \"Remove\"，则隐藏行不会被输出；如果该值为 \"Hidden\"，行会被输出，但仍保持隐藏，默认值为 \"Hidden\"。

参见 [HtmlHiddenRowDisplayType](../../com.aspose.cells/htmlhiddenrowdisplaytype)。

**Returns:**
int
### getHideOverflowWrappedText() {#getHideOverflowWrappedText--}
```
public boolean getHideOverflowWrappedText()
```


指示在单元格格式设置为自动换行时是否隐藏溢出文本。默认值为 false。

**Returns:**
boolean
### getHtmlCrossStringType() {#getHtmlCrossStringType--}
```
public int getHtmlCrossStringType()
```


指示在将 Excel 文件保存为 html 格式时，跨单元格字符串是否以与 MS Excel 相同的方式显示。默认值为 Default，因此对于跨单元格字符串，Aspose.Cells 与 MS Excel 创建的 html 文件差别不大。但在生成大型 html 文件时，将值设为 Cross 的性能比设为 Default 或 Fit2Cell 快数倍。

参见 [HtmlCrossType](../../com.aspose.cells/htmlcrosstype)。

**Returns:**
int
### getHtmlVersion() {#getHtmlVersion--}
```
public int getHtmlVersion()
```


指定保存为 HTML 格式时应使用的 HTML 标准版本。默认值为 HtmlVersion.Default。

参见 [HtmlVersion](../../com.aspose.cells/htmlversion)。

**Returns:**
int
### getIgnoreInvisibleShapes() {#getIgnoreInvisibleShapes--}
```
public boolean getIgnoreInvisibleShapes()
```


指示是否导出不可见的形状。

**Remarks**

默认值为 false。

**Returns:**
boolean
### getImageOptions() {#getImageOptions--}
```
public ImageOrPrintOptions getImageOptions()
```


在导出之前获取 ImageOrPrintOptions 对象。

**Returns:**
[ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions)
### getImageScalable() {#getImageScalable--}
```
public boolean getImageScalable()
```


指示在使用可伸缩单位描述列宽时，是否使用可伸缩单位描述图像宽度。默认值为 true。

**Returns:**
boolean
### getLayoutMode() {#getLayoutMode--}
```
public int getLayoutMode()
```


获取保存为 HTML 时的布局模式。默认值为 [HtmlLayoutMode.NORMAL](../../com.aspose.cells/htmllayoutmode\#NORMAL)。

参见 [HtmlLayoutMode](../../com.aspose.cells/htmllayoutmode)。

**Returns:**
int
### getLinkTargetType() {#getLinkTargetType--}
```
public int getLinkTargetType()
```


指示 `<a>` 链接中 target 属性的类型。默认值为 HtmlLinkTargetType.Parent。

参见 [HtmlLinkTargetType](../../com.aspose.cells/htmllinktargettype)。

**Returns:**
int
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


指示在保存文件之前是否合并条件格式和验证的区域。

**Remarks**

默认值为 false。

**Returns:**
boolean
### getMergeEmptyTdForcely() {#getMergeEmptyTdForcely--}
```
public boolean getMergeEmptyTdForcely()
```


指示在导出文件为 html 时是否强制合并空的 TD 元素。将该值设为 true 后，html 文件的大小将显著减小。默认值为 false。如果您希望将 html 文件导入 Excel，或在保存为 html 时导出完整的网格线，请保持默认值。

**Returns:**
boolean
### getMergeEmptyTdType() {#getMergeEmptyTdType--}
```
public int getMergeEmptyTdType()
```


合并连续空单元格（空 td 元素）的选项。默认值为 MergeEmptyTdType.Default。

参见 [MergeEmptyTdType](../../com.aspose.cells/mergeemptytdtype)。

**Returns:**
int
### getOfficeMathOutputMode() {#getOfficeMathOutputMode--}
```
public int getOfficeMathOutputMode()
```


指示 OfficeMath 对象如何导出为 HTML，默认值为 Image。

参见 [HtmlOfficeMathOutputType](../../com.aspose.cells/htmlofficemathoutputtype)。

**Returns:**
int
### getPageTitle() {#getPageTitle--}
```
public String getPageTitle()
```


HTML 页面标题。仅用于保存为 html 流。

**Returns:**
java.lang.String
### getParseHtmlTagInCell() {#getParseHtmlTagInCell--}
```
public boolean getParseHtmlTagInCell()
```


指示单元格中的 html 标记（例如 `<div></div>`）是应解析为单元格值还是保持原样。默认值为 true。

**Returns:**
boolean
### getPresentationPreference() {#getPresentationPreference--}
```
public boolean getPresentationPreference()
```


指示 html 或 mht 文件是否为首选展示方式。默认值为 false。如果希望获得更美观的展示，请将该值设为 true。

**Returns:**
boolean
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```


指示是否缓存图表的最新数据。

**Returns:**
boolean
### getSaveAsSingleFile() {#getSaveAsSingleFile--}
```
public boolean getSaveAsSingleFile()
```


指示是否将 html 保存为单个文件。默认值为 false。

**Remarks**

如果工作簿中有多个工作表或其他必需资源（如图片），通常这些工作表和资源需要保存为独立文件。某些场景下，为了便于传输，用户可能只需要一个结果文件。此时，用户可以将此属性设为 true。

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


获取保存的文件格式。

参见 [SaveFormat](../../com.aspose.cells/saveformat)。

**Returns:**
int
### getSheetSet() {#getSheetSet--}
```
public SheetSet getSheetSet()
```


获取要渲染的工作表。默认是工作簿中所有可见工作表：[SheetSet.getVisible()](../../com.aspose.cells/sheetset\\#getVisible--)。

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getShowAllSheets() {#getShowAllSheets--}
```
public boolean getShowAllSheets()
```


指示在保存为单个 HTML 文件时是否显示所有工作表。

**Remarks**

仅在 [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) 为 True 时有效。

**Returns:**
boolean
### getSortExternalNames() {#getSortExternalNames--}
```
public boolean getSortExternalNames()
```


指示在保存文件之前是否对外部已定义名称进行排序。

**Returns:**
boolean
### getSortNames() {#getSortNames--}
```
public boolean getSortNames()
```


指示在保存文件之前是否对已定义名称进行排序。

**Returns:**
boolean
### getSpaceMode() {#getSpaceMode--}
```
public int getSpaceMode()
```


指示在 HTML 输出中空格的渲染方式。此选项目前仅适用于数值格式（例如会计格式）。默认值为 [HtmlSpaceMode.CSS](../../com.aspose.cells/htmlspacemode\\#CSS)。

参见 [HtmlSpaceMode](../../com.aspose.cells/htmlspacemode)。

**Returns:**
int
### getStreamProvider() {#getStreamProvider--}
```
public IStreamProvider getStreamProvider()
```


获取用于导出对象的 IStreamProvider。

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getTableCssId() {#getTableCssId--}
```
public String getTableCssId()
```


获取类型 css 名称的前缀，如 tr、col、td 等，它们位于具有特定 TableCssId 属性的 table 元素中。默认值为 \"\"。

**Returns:**
java.lang.String
### getUpdateSmartArt() {#getUpdateSmartArt--}
```
public boolean getUpdateSmartArt()
```


指示是否更新 Smart Art 设置。默认值为 false。

**Remarks**

仅在调用 Shape.GetResultOfSmartArt() 方法且模板文件中存在缓存形状后生效。

**Returns:**
boolean
### getValidateMergedAreas() {#getValidateMergedAreas--}
```
public boolean getValidateMergedAreas()
```


指示在保存文件之前是否验证合并的单元格。

**Remarks**

默认值为 false。

**Returns:**
boolean
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


获取警告回调。

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### getWidthScalable() {#getWidthScalable--}
```
public boolean getWidthScalable()
```


指示是否以比例单位导出列宽到 html。默认值为 false。

**Returns:**
boolean
### getWorksheetScalable() {#getWorksheetScalable--}
```
public boolean getWorksheetScalable()
```


指示在将文件保存为 HTML 时是否通过工作表缩放级别对 HTML 进行放大或缩小，默认值为 false。

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBorderCollapsed() {#isBorderCollapsed--}
```
public boolean isBorderCollapsed()
```


指示表格边框是否折叠。默认值为 true。

**Returns:**
boolean
### isExpImageToTempDir() {#isExpImageToTempDir--}
```
public boolean isExpImageToTempDir()
```


指示是否将图像文件导出到临时目录。仅用于保存为 html 流。

**Returns:**
boolean
### isExportComments() {#isExportComments--}
```
public boolean isExportComments()
```


指示在将文件保存为 HTML 时是否导出注释，默认值为 false。

**Returns:**
boolean
### isFullPathLink() {#isFullPathLink--}
```
public boolean isFullPathLink()
```


指示在 sheet00x.htm、filelist.xml 和 tabstrip.htm 中是否使用完整路径链接。默认值为 false。

**Returns:**
boolean
### isIECompatible() {#isIECompatible--}
```
public boolean isIECompatible()
```


指示输出的 HTML 是否兼容 IE 浏览器。默认值为 false。

**Returns:**
boolean
### isJsBrowserCompatible() {#isJsBrowserCompatible--}
```
public boolean isJsBrowserCompatible()
```


指示 JavaScript 是否兼容不支持 JavaScript 的浏览器。默认值为 true。

**Returns:**
boolean
### isMobileCompatible() {#isMobileCompatible--}
```
public boolean isMobileCompatible()
```


指示输出的 HTML 是否兼容移动设备。默认值为 false。

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




### setAddGenericFont(boolean value) {#setAddGenericFont-boolean-}
```
public void setAddGenericFont(boolean value)
```


指示是否向 CSS font-family 添加通用字体。默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAddTooltipText(boolean value) {#setAddTooltipText-boolean-}
```
public void setAddTooltipText(boolean value)
```


指示在数据无法完整显示时是否添加工具提示文本。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAttachedFilesDirectory(String value) {#setAttachedFilesDirectory-java.lang.String-}
```
public void setAttachedFilesDirectory(String value)
```


附加文件将保存到的目录。仅用于保存为 html 流。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setAttachedFilesUrlPrefix(String value) {#setAttachedFilesUrlPrefix-java.lang.String-}
```
public void setAttachedFilesUrlPrefix(String value)
```


指定附加文件（如 html 文件中的图像）的 Url 前缀。仅用于保存为 html 流。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setBorderCollapsed(boolean value) {#setBorderCollapsed-boolean-}
```
public void setBorderCollapsed(boolean value)
```


指示表格边框是否折叠。默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```


用于临时文件的文件夹，可用作数据缓存。

**Remarks**

如果未指定文件夹，则其默认值为 [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--)。如果其默认值为 null 或为空，或已指定为 null 或为空，则在保存工作簿时不会使用缓存文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setCalculateFormula(boolean value) {#setCalculateFormula-boolean-}
```
public void setCalculateFormula(boolean value)
```


指示是否在保存 html 文件之前计算公式。

**Remarks**

默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setCellCssPrefix(String value) {#setCellCssPrefix-java.lang.String-}
```
public void setCellCssPrefix(String value)
```


设置 CSS 名称的前缀，默认值为 ""。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setCellNameAttribute(String value) {#setCellNameAttribute-java.lang.String-}
```
public void setCellNameAttribute(String value)
```


指定用于写入 CellName 的属性。（例如，如果值为 "id"，则单元格 "A1" 的输出将是：<td id='A1'>）。默认值为 null。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


是否在用户修改单元格相关对象时检查 Excel 文件的限制。例如，Excel 不允许输入超过 32K 的字符串值。当您输入超过 32K 的值时，它将被截断。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setClearData(boolean value) {#setClearData-boolean-}
```
public void setClearData(boolean value)
```


在保存文件后使工作簿为空。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setCreateDirectory(boolean value) {#setCreateDirectory-boolean-}
```
public void setCreateDirectory(boolean value)
```


如果为 true 且目录不存在，目录将在保存文件之前自动创建。

**Remarks**

默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setCssStyles(String value) {#setCssStyles-java.lang.String-}
```
public void setCssStyles(String value)
```


设置格式化器的附加 css 样式。仅在 [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\\#getSaveAsSingleFile--) 为 True 时生效。CssStyles=\"body \\\{ padding: 5px \\\}\";

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setDataBarRenderMode(int value) {#setDataBarRenderMode-int-}
```
public void setDataBarRenderMode(int value)
```


表示在将 Excel 文件转换为 html 文件时渲染 DataBar 的模式。默认值为 [DataBarRenderMode.BACKGROUND\_COLOR](../../com.aspose.cells/databarrendermode\#BACKGROUND-COLOR)。

参见 [DataBarRenderMode](../../com.aspose.cells/databarrendermode)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```


指定导出 html 时的默认字体名称，当样式的字体不存在时将使用默认字体；如果此属性为 null，Aspose.Cells 将使用与原始字体同一系列的通用字体，默认值为 null。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setDisableCss(boolean value) {#setDisableCss-boolean-}
```
public void setDisableCss(boolean value)
```


指示是否仅应用内联样式，而不依赖 CSS。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setDisableDownlevelRevealedComments(boolean value) {#setDisableDownlevelRevealedComments-boolean-}
```
public void setDisableDownlevelRevealedComments(boolean value)
```


指示在导出文件为 html 时是否禁用 Downlevel-revealed 条件注释，默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEmbeddedFontType(int value) {#setEmbeddedFontType-int-}
```
public void setEmbeddedFontType(int value)
```


设置嵌入字体文件到 html 文件的类型。默认值为 [HtmlEmbeddedFontType.NONE](../../com.aspose.cells/htmlembeddedfonttype\\#NONE)，表示不在 html 中嵌入任何字体。

参见 [HtmlEmbeddedFontType](../../com.aspose.cells/htmlembeddedfonttype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setEnableCssCustomProperties(boolean value) {#setEnableCssCustomProperties-boolean-}
```
public void setEnableCssCustomProperties(boolean value)
```


通过使用 CSS 自定义属性优化 html 的输出。例如，在同一 base64 图像出现多次的情况下，使用自定义属性只需保存一次图像数据，从而提升生成的 html 性能。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEncodeEntityAsCode(boolean value) {#setEncodeEntityAsCode-boolean-}
```
public void setEncodeEntityAsCode(boolean value)
```


指示是否将 html 字符实体替换为十进制代码。（例如，"&nbsp;" 被替换为 "&\#160;"）。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```


如果未设置，则使用 Encoding.UTF8 作为默认编码类型。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setEncryptDocumentProperties(boolean value) {#setEncryptDocumentProperties-boolean-}
```
public void setEncryptDocumentProperties(boolean value)
```


指示在保存为 .xls 文件时是否加密文档属性。默认值为 true。

**Remarks**

仅适用于 .xls、xlsx、xlsb 和 xlsm 文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExcludeUnusedStyles(boolean value) {#setExcludeUnusedStyles-boolean-}
```
public void setExcludeUnusedStyles(boolean value)
```


指示是否排除未使用的样式。对于生成的 html 文件，排除未使用的样式可以在不影响视觉效果的前提下降小文件大小。因此此属性的默认值为 true。如果用户需要在工作簿中保留所有样式以供生成的 html 使用（例如用户稍后需要从生成的 html 恢复工作簿），请将此属性设为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExpImageToTempDir(boolean value) {#setExpImageToTempDir-boolean-}
```
public void setExpImageToTempDir(boolean value)
```


指示是否将图像文件导出到临时目录。仅用于保存为 html 流。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExportActiveWorksheetOnly(boolean value) {#setExportActiveWorksheetOnly-boolean-}
```
public void setExportActiveWorksheetOnly(boolean value)
```


指示是否仅导出活动工作表到 html 文件。如果为 true，则仅导出活动工作表；如果为 false，则导出整个工作簿。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExportArea(CellArea value) {#setExportArea-com.aspose.cells.CellArea-}
```
public void setExportArea(CellArea value)
```


设置当前活动工作表的导出 CellArea。如果设置此属性，当前活动工作表的打印区域将被省略。保存为 html 时仅导出指定区域。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [CellArea](../../com.aspose.cells/cellarea) |  |

### setExportBogusRowData(boolean value) {#setExportBogusRowData-boolean-}
```
public void setExportBogusRowData(boolean value)
```


指示是否导出虚假的底部行数据。默认值为 true。如果希望将 html 或 mht 文件导入 Excel，请保持默认值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExportCellCoordinate(boolean value) {#setExportCellCoordinate-boolean-}
```
public void setExportCellCoordinate(boolean value)
```


指示在保存文件为 html 时是否导出非空单元格的 Excel 坐标。默认值为 false。如果希望将生成的 html 导入 Excel，请保持默认值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExportComments(boolean value) {#setExportComments-boolean-}
```
public void setExportComments(boolean value)
```


指示在将文件保存为 HTML 时是否导出注释，默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExportCommentsType(int value) {#setExportCommentsType-int-}
```
public void setExportCommentsType(int value)
```


表示导出注释到 html 文件的类型。

参见 [PrintCommentsType](../../com.aspose.cells/printcommentstype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setExportDataOptions(int value) {#setExportDataOptions-int-}
```
public void setExportDataOptions(int value)
```


指示导出 html 文件数据的规则。默认值为 All。

参见 [HtmlExportDataOptions](../../com.aspose.cells/htmlexportdataoptions)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setExportDocumentProperties(boolean value) {#setExportDocumentProperties-boolean-}
```
public void setExportDocumentProperties(boolean value)
```


指示是否导出文档属性。默认值为 true。如果要将 html 或 mht 文件导入到 excel，请保持默认值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExportExtraHeadings(boolean value) {#setExportExtraHeadings-boolean-}
```
public void setExportExtraHeadings(boolean value)
```


指示当文本长度超过最大显示列时是否导出额外的标题。默认值为 false。如果希望将 html 文件导入 Excel，请保持默认值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExportFormula(boolean value) {#setExportFormula-boolean-}
```
public void setExportFormula(boolean value)
```


指示在保存文件为 html 时是否导出公式。默认值为 true。如果希望将生成的 html 导入 Excel，请保持默认值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExportFrameScriptsAndProperties(boolean value) {#setExportFrameScriptsAndProperties-boolean-}
```
public void setExportFrameScriptsAndProperties(boolean value)
```


指示是否导出框架脚本和文档属性。默认值为 true。如果希望将 html 或 mht 文件导入 Excel，请保持默认值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExportGridLines(boolean value) {#setExportGridLines-boolean-}
```
public void setExportGridLines(boolean value)
```


指示是否导出网格线。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExportHeadings(boolean value) {#setExportHeadings-boolean-}
```
public void setExportHeadings(boolean value)
```


指示在保存为 HTML 文件时是否导出工作表的行列标题。

**Remarks**

注意：此成员现已过时。请改用 HtmlSaveOptions.ExportRowColumnHeadings 属性。此属性将在自 2022 年 6 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExportHiddenWorksheet(boolean value) {#setExportHiddenWorksheet-boolean-}
```
public void setExportHiddenWorksheet(boolean value)
```


指示是否导出隐藏工作表的内容。默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExportImagesAsBase64(boolean value) {#setExportImagesAsBase64-boolean-}
```
public void setExportImagesAsBase64(boolean value)
```


指定图像是否以 Base64 格式保存到 HTML、MHTML 或 EPUB。

**Remarks**

当此属性设置为 true 时，图像数据直接导出到 img 元素上，不会创建单独的文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExportNamedRangeAnchors(boolean value) {#setExportNamedRangeAnchors-boolean-}
```
public void setExportNamedRangeAnchors(boolean value)
```


指示在保存为 HTML 时是否导出命名范围的锚点元素。默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExportObjectListener(IExportObjectListener value) {#setExportObjectListener-com.aspose.cells.IExportObjectListener-}
```
public void setExportObjectListener(IExportObjectListener value)
```


设置用于导出对象的 ExportObjectListener。

**Remarks**

注意：此属性已过时。请改用 HtmlSaveOptions.IStreamProvider 属性。该属性将在自 2015 年 8 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [IExportObjectListener](../../com.aspose.cells/iexportobjectlistener) |  |

### setExportPageFooters(boolean value) {#setExportPageFooters-boolean-}
```
public void setExportPageFooters(boolean value)
```


指示是否导出页面标题。

**Remarks**

仅在 [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) 为 True 时有效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExportPageHeaders(boolean value) {#setExportPageHeaders-boolean-}
```
public void setExportPageHeaders(boolean value)
```


指示是否导出页面标题。

**Remarks**

仅在 [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) 为 True 时有效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExportPrintAreaOnly(boolean value) {#setExportPrintAreaOnly-boolean-}
```
public void setExportPrintAreaOnly(boolean value)
```


指示是否仅导出打印区域到 HTML 文件。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExportRowColumnHeadings(boolean value) {#setExportRowColumnHeadings-boolean-}
```
public void setExportRowColumnHeadings(boolean value)
```


指示在保存为 HTML 文件时是否导出工作表的行列标题。

**Remarks**

默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExportSimilarBorderStyle(boolean value) {#setExportSimilarBorderStyle-boolean-}
```
public void setExportSimilarBorderStyle(boolean value)
```


指示在浏览器不支持的情况下是否导出相似的边框样式。如果您想将 html 或 mht 文件导入到 Excel，请保持默认值。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExportSingleTab(boolean value) {#setExportSingleTab-boolean-}
```
public void setExportSingleTab(boolean value)
```


指示当文件仅包含一个工作表时是否导出单个标签页。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExportWorkbookProperties(boolean value) {#setExportWorkbookProperties-boolean-}
```
public void setExportWorkbookProperties(boolean value)
```


指示是否导出工作簿属性。默认值为 true。如果您想将 html 或 mht 文件导入 Excel，请保持默认值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExportWorksheetCSSSeparately(boolean value) {#setExportWorksheetCSSSeparately-boolean-}
```
public void setExportWorksheetCSSSeparately(boolean value)
```


指示是否单独导出工作表 CSS。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExportWorksheetProperties(boolean value) {#setExportWorksheetProperties-boolean-}
```
public void setExportWorksheetProperties(boolean value)
```


指示是否导出工作表属性。默认值为 true。如果您想将 html 或 mht 文件导入 Excel，请保持默认值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setFilePathProvider(IFilePathProvider value) {#setFilePathProvider-com.aspose.cells.IFilePathProvider-}
```
public void setFilePathProvider(IFilePathProvider value)
```


设置用于单独导出工作表到 HTML 的 IFilePathProvider。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [IFilePathProvider](../../com.aspose.cells/ifilepathprovider) |  |

### setFormatDataIgnoreColumnWidth(boolean value) {#setFormatDataIgnoreColumnWidth-boolean-}
```
public void setFormatDataIgnoreColumnWidth(boolean value)
```


指示当内容溢出列时是否显示单元格的完整格式化数据。如果为 true，则忽略列宽并导出单元格的全部数据；如果为 false，则数据的导出方式与 Excel 相同。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setFullPathLink(boolean value) {#setFullPathLink-boolean-}
```
public void setFullPathLink(boolean value)
```


指示在 sheet00x.htm、filelist.xml 和 tabstrip.htm 中是否使用完整路径链接。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setHiddenColDisplayType(int value) {#setHiddenColDisplayType-int-}
```
public void setHiddenColDisplayType(int value)
```


在 Excel 中隐藏列（此列宽度为 0），在保存为 HTML 格式之前，如果 HtmlHiddenColDisplayType 为 \"Remove\"，则隐藏列不会被输出；如果该值为 \"Hidden\"，列会被输出，但仍保持隐藏，默认值为 \"Hidden\"。

参见 [HtmlHiddenColDisplayType](../../com.aspose.cells/htmlhiddencoldisplaytype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setHiddenRowDisplayType(int value) {#setHiddenRowDisplayType-int-}
```
public void setHiddenRowDisplayType(int value)
```


在 Excel 中隐藏行（此行高度为 0），在保存为 HTML 格式之前，如果 HtmlHiddenRowDisplayType 为 \"Remove\"，则隐藏行不会被输出；如果该值为 \"Hidden\"，行会被输出，但仍保持隐藏，默认值为 \"Hidden\"。

参见 [HtmlHiddenRowDisplayType](../../com.aspose.cells/htmlhiddenrowdisplaytype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setHideOverflowWrappedText(boolean value) {#setHideOverflowWrappedText-boolean-}
```
public void setHideOverflowWrappedText(boolean value)
```


指示在单元格格式设置为自动换行时是否隐藏溢出文本。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setHtmlCrossStringType(int value) {#setHtmlCrossStringType-int-}
```
public void setHtmlCrossStringType(int value)
```


指示在将 Excel 文件保存为 html 格式时，跨单元格字符串是否以与 MS Excel 相同的方式显示。默认值为 Default，因此对于跨单元格字符串，Aspose.Cells 与 MS Excel 创建的 html 文件差别不大。但在生成大型 html 文件时，将值设为 Cross 的性能比设为 Default 或 Fit2Cell 快数倍。

参见 [HtmlCrossType](../../com.aspose.cells/htmlcrosstype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setHtmlVersion(int value) {#setHtmlVersion-int-}
```
public void setHtmlVersion(int value)
```


指定保存为 HTML 格式时应使用的 HTML 标准版本。默认值为 HtmlVersion.Default。

参见 [HtmlVersion](../../com.aspose.cells/htmlversion)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setIECompatible(boolean value) {#setIECompatible-boolean-}
```
public void setIECompatible(boolean value)
```


指示输出的 HTML 是否兼容 IE 浏览器。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setIgnoreInvisibleShapes(boolean value) {#setIgnoreInvisibleShapes-boolean-}
```
public void setIgnoreInvisibleShapes(boolean value)
```


指示是否导出不可见的形状。

**Remarks**

默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setImageScalable(boolean value) {#setImageScalable-boolean-}
```
public void setImageScalable(boolean value)
```


指示在使用可伸缩单位描述列宽时，是否使用可伸缩单位描述图像宽度。默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setJsBrowserCompatible(boolean value) {#setJsBrowserCompatible-boolean-}
```
public void setJsBrowserCompatible(boolean value)
```


指示 JavaScript 是否兼容不支持 JavaScript 的浏览器。默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setLayoutMode(int value) {#setLayoutMode-int-}
```
public void setLayoutMode(int value)
```


设置保存为 HTML 时的布局模式。默认值为 [HtmlLayoutMode.NORMAL](../../com.aspose.cells/htmllayoutmode\\#NORMAL)。

参见 [HtmlLayoutMode](../../com.aspose.cells/htmllayoutmode)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setLinkTargetType(int value) {#setLinkTargetType-int-}
```
public void setLinkTargetType(int value)
```


指示 `<a>` 链接中 target 属性的类型。默认值为 HtmlLinkTargetType.Parent。

参见 [HtmlLinkTargetType](../../com.aspose.cells/htmllinktargettype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setMergeAreas(boolean value) {#setMergeAreas-boolean-}
```
public void setMergeAreas(boolean value)
```


指示在保存文件之前是否合并条件格式和验证的区域。

**Remarks**

默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setMergeEmptyTdForcely(boolean value) {#setMergeEmptyTdForcely-boolean-}
```
public void setMergeEmptyTdForcely(boolean value)
```


指示在导出文件为 html 时是否强制合并空的 TD 元素。将该值设为 true 后，html 文件的大小将显著减小。默认值为 false。如果您希望将 html 文件导入 Excel，或在保存为 html 时导出完整的网格线，请保持默认值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setMergeEmptyTdType(int value) {#setMergeEmptyTdType-int-}
```
public void setMergeEmptyTdType(int value)
```


合并连续空单元格（空 td 元素）的选项。默认值为 MergeEmptyTdType.Default。

参见 [MergeEmptyTdType](../../com.aspose.cells/mergeemptytdtype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setMobileCompatible(boolean value) {#setMobileCompatible-boolean-}
```
public void setMobileCompatible(boolean value)
```


指示输出的 HTML 是否兼容移动设备。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setOfficeMathOutputMode(int value) {#setOfficeMathOutputMode-int-}
```
public void setOfficeMathOutputMode(int value)
```


指示 OfficeMath 对象如何导出为 HTML，默认值为 Image。

参见 [HtmlOfficeMathOutputType](../../com.aspose.cells/htmlofficemathoutputtype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setPageTitle(String value) {#setPageTitle-java.lang.String-}
```
public void setPageTitle(String value)
```


HTML 页面标题。仅用于保存为 html 流。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setParseHtmlTagInCell(boolean value) {#setParseHtmlTagInCell-boolean-}
```
public void setParseHtmlTagInCell(boolean value)
```


指示单元格中的 html 标记（例如 `<div></div>`）是应解析为单元格值还是保持原样。默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setPresentationPreference(boolean value) {#setPresentationPreference-boolean-}
```
public void setPresentationPreference(boolean value)
```


指示 html 或 mht 文件是否为首选展示方式。默认值为 false。如果希望获得更美观的展示，请将该值设为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


指示是否缓存图表的最新数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSaveAsSingleFile(boolean value) {#setSaveAsSingleFile-boolean-}
```
public void setSaveAsSingleFile(boolean value)
```


指示是否将 html 保存为单个文件。默认值为 false。

**Remarks**

如果工作簿中有多个工作表或其他必需资源（如图片），通常这些工作表和资源需要保存为独立文件。某些场景下，为了便于传输，用户可能只需要一个结果文件。此时，用户可以将此属性设为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSheetSet(SheetSet value) {#setSheetSet-com.aspose.cells.SheetSet-}
```
public void setSheetSet(SheetSet value)
```


设置要渲染的工作表。默认是工作簿中所有可见工作表：[SheetSet.getVisible()](../../com.aspose.cells/sheetset\\#getVisible--)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [SheetSet](../../com.aspose.cells/sheetset) |  |

### setShowAllSheets(boolean value) {#setShowAllSheets-boolean-}
```
public void setShowAllSheets(boolean value)
```


指示在保存为单个 HTML 文件时是否显示所有工作表。

**Remarks**

仅在 [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) 为 True 时有效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSortExternalNames(boolean value) {#setSortExternalNames-boolean-}
```
public void setSortExternalNames(boolean value)
```


指示在保存文件之前是否对外部已定义名称进行排序。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSortNames(boolean value) {#setSortNames-boolean-}
```
public void setSortNames(boolean value)
```


指示在保存文件之前是否对已定义名称进行排序。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSpaceMode(int value) {#setSpaceMode-int-}
```
public void setSpaceMode(int value)
```


指示在 HTML 输出中空格的渲染方式。此选项目前仅适用于数值格式（例如会计格式）。默认值为 [HtmlSpaceMode.CSS](../../com.aspose.cells/htmlspacemode\\#CSS)。

参见 [HtmlSpaceMode](../../com.aspose.cells/htmlspacemode)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setStreamProvider(IStreamProvider value) {#setStreamProvider-com.aspose.cells.IStreamProvider-}
```
public void setStreamProvider(IStreamProvider value)
```


设置用于导出对象的 IStreamProvider。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setTableCssId(String value) {#setTableCssId-java.lang.String-}
```
public void setTableCssId(String value)
```


设置类型 css 名称的前缀，如 tr、col、td 等，它们位于具有特定 TableCssId 属性的 table 元素中。默认值为 \"\"。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setUpdateSmartArt(boolean value) {#setUpdateSmartArt-boolean-}
```
public void setUpdateSmartArt(boolean value)
```


指示是否更新 Smart Art 设置。默认值为 false。

**Remarks**

仅在调用 Shape.GetResultOfSmartArt() 方法且模板文件中存在缓存形状后生效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setValidateMergedAreas(boolean value) {#setValidateMergedAreas-boolean-}
```
public void setValidateMergedAreas(boolean value)
```


指示在保存文件之前是否验证合并的单元格。

**Remarks**

默认值为 false。

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

### setWidthScalable(boolean value) {#setWidthScalable-boolean-}
```
public void setWidthScalable(boolean value)
```


指示是否以比例单位导出列宽到 html。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setWorksheetScalable(boolean value) {#setWorksheetScalable-boolean-}
```
public void setWorksheetScalable(boolean value)
```


指示在将文件保存为 HTML 时是否通过工作表缩放级别对 HTML 进行放大或缩小，默认值为 false。

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

