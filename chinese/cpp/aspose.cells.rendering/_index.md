---
title: "Aspose::Cells::Rendering 命名空间"
linktitle: "Aspose::Cells::Rendering"
second_title: "Aspose.Cells for C++ API 参考"
description: "如何在 C++ 中使用 Aspose::Cells::Rendering 命名空间。"
type: docs
weight: 2200
url: /zh/cpp/aspose.cells.rendering/
---



## 类

| 类 | 描述 |
| --- | --- |
| [CustomRenderSettings](./customrendersettings/) | 表示渲染期间的自定义设置。 |
| [DrawObject](./drawobject/) | [DrawObject](./drawobject/) 将在渲染时被初始化并返回。 |
| [DrawObjectEventHandler](./drawobjecteventhandler/) | 用于在渲染时获取 [DrawObject](./drawobject/) 和 Bound 的接口。 |
| [ImageOrPrintOptions](./imageorprintoptions/) | 允许在将工作表渲染为图像、打印工作表或将图表渲染为图像时指定选项。 |
| [IPageSavingCallback](./ipagesavingcallback/) | 控制/指示页面保存过程的进度。 |
| [PageEndSavingArgs](./pageendsavingargs/) | 页面结束保存过程的信息。 |
| [PageSavingArgs](./pagesavingargs/) | 页面保存过程的信息。 |
| [PageStartSavingArgs](./pagestartsavingargs/) | 页面开始保存过程的信息。 |
| [PdfBookmarkEntry](./pdfbookmarkentry/) | [PdfBookmarkEntry](./pdfbookmarkentry/) 是 PDF 书签中的一个条目。如果当前实例的 Text 属性为 null 或 "", 则当前实例将被隐藏，子项将插入到当前层级。 |
| [RenderingFont](./renderingfont/) | [Font](../aspose.cells/font/) 用于渲染。 |
| [RenderingWatermark](./renderingwatermark/) | 渲染用水印。 |
| [SheetPrintingPreview](./sheetprintingpreview/) | [Worksheet](../aspose.cells/worksheet/) 打印预览。 |
| [SheetRender](./sheetrender/) | 表示工作表渲染器，可将工作表渲染为各种图像（如 BMP、PNG、JPEG、TIFF 等）。此类的构造函数必须在修改页面设置和单元格样式后使用。 |
| [SheetSet](./sheetset/) | 描述一组工作表。 |
| [SvgImageOptions](./svgimageoptions/) | 生成 Svg 图像的选项。 |
| [WorkbookPrintingPreview](./workbookprintingpreview/) | [Workbook](../aspose.cells/workbook/) 打印预览。 |
| [WorkbookRender](./workbookrender/) | 表示一个 [Workbook](../aspose.cells/workbook/) 渲染器。此类的构造函数必须在修改页面设置和单元格样式后使用。 |
## Enums

| 枚举 | 描述 |
| --- | --- |
| [ColorDepth](./colordepth/) | 枚举 TIFF 图像的位深类型。 |
| [CommentTitleType](./commenttitletype/) | 表示在渲染时评论设置为在工作表末尾显示时的评论标题类型。 |
| [DataBarRenderMode](./databarrendermode/) | 表示 [DataBar](../aspose.cells/databar/) 渲染模式。 |
| [DrawObjectEnum](./drawobjectenum/) | 指示 [Cell](../aspose.cells/cell/) 或 [DrawObject](./drawobject/) 的图像。 |
| [ExcelRenderingBehavior](./excelrenderingbehavior/) | 指定在渲染工作簿时要应用的 Excel 特定渲染行为。 |
| [HtmlEmbeddedFontType](./htmlembeddedfonttype/) | 表示 HTML 中的嵌入字体类型。 |
| [HtmlLayoutMode](./htmllayoutmode/) | 表示 HTML 渲染的布局模式。 |
| [HtmlParagraphLayoutMode](./htmlparagraphlayoutmode/) | 指定在加载 HTML 时 <p> 元素的渲染方式。 |
| [HtmlSpaceMode](./htmlspacemode/) | 指定在生成的 HTML 中空白字符的表示方式。 |
| [ImageBinarizationMethod](./imagebinarizationmethod/) | 指定用于二值化图像的方法。 |
| [PdfCompliance](./pdfcompliance/) | 允许用户设置 PDF 转换的兼容性。 |
| [PdfCompressionCore](./pdfcompressioncore/) | 指定对 PDF 文件中除图像外的所有内容应用的压缩类型。 |
| [PdfCustomPropertiesExport](./pdfcustompropertiesexport/) | 指定 CustomDocumentPropertyCollection 导出到 PDF 文件的方式。 |
| [PdfFontEncoding](./pdffontencoding/) | 表示 PDF 嵌入字体的编码。 |
| [PdfOptimizationType](./pdfoptimizationtype/) | 指定一种优化类型。 |
| [PdfZoomBehavior](./pdfzoombehavior/) | 指定打开生成的 PDF 文档时的初始视图模式。 |
| [SvgEmbeddedFontType](./svgembeddedfonttype/) | 表示 SVG 图像中的嵌入字体类型。 |
| [TiffCompression](./tiffcompression/) | 指定在将图像保存为 TIFF 格式文件时要应用的压缩类型。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| ExcelRenderingBehavior operator&(ExcelRenderingBehavior a, ExcelRenderingBehavior b) |  |
