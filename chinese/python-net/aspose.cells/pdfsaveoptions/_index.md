---
title: PdfSaveOptions类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 1180
url: /zh/python-net/aspose.cells/pdfsaveoptions/
is_root: false
---
## PdfSaveOptions类
代表保存pdf文件的选项。



**继承：** [PdfSaveOptions](/cells/python-net/aspose.cells/pdfsaveoptions) → 
[PaginatedSaveOptions](/cells/python-net/aspose.cells/paginatedsaveoptions) → 
[SaveOptions](/cells/zh/python-net/aspose.cells/saveoptions)



PdfSaveOptions 类型公开了以下成员：

### 构造器
|构造器|描述|
| :- | :- |
| [PdfSaveOptions()](/cells/zh/python-net/aspose.cells/pdfsaveoptions/__init__/#) |创建用于保存 pdf 文件的选项。|


### 特性
|属性|描述|
| :- | :- |
| [save_format](/cells/zh/python-net/aspose.cells/pdfsaveoptions/save_format) |获取保存文件格式。|
| [clear_data](/cells/zh/python-net/aspose.cells/pdfsaveoptions/clear_data) |保存文件后将工作簿清空。|
| [cached_file_folder](/cells/zh/python-net/aspose.cells/pdfsaveoptions/cached_file_folder) |缓存文件夹用于存储一些大数据。|
| [validate_merged_areas](/cells/zh/python-net/aspose.cells/pdfsaveoptions/validate_merged_areas) |指示是否在保存文件之前验证合并的单元格。|
| [merge_areas](/cells/zh/python-net/aspose.cells/pdfsaveoptions/merge_areas) |指示是否在保存文件之前合并条件格式和验证区域。|
| [create_directory](/cells/zh/python-net/aspose.cells/pdfsaveoptions/create_directory) |如果为 true 并且目录不存在，则在保存文件之前会自动创建目录。|
| [sort_names](/cells/zh/python-net/aspose.cells/pdfsaveoptions/sort_names) |指示是否在保存文件之前对定义的名称进行排序。|
| [sort_external_names](/cells/zh/python-net/aspose.cells/pdfsaveoptions/sort_external_names) |指示是否在保存文件之前对外部定义的名称进行排序。|
| [refresh_chart_cache](/cells/zh/python-net/aspose.cells/pdfsaveoptions/refresh_chart_cache) |指示是否刷新图表缓存数据|
| [warning_callback](/cells/zh/python-net/aspose.cells/pdfsaveoptions/warning_callback) |获取或设置警告回调。|
| [update_smart_art](/cells/zh/python-net/aspose.cells/pdfsaveoptions/update_smart_art) |指示是否更新智能艺术设置。<br/>默认值为假。|
| [default_font](/cells/zh/python-net/aspose.cells/pdfsaveoptions/default_font) |当Excel中的字符是Unicode且未在单元格样式中设置正确的字体时，<br/>它们可能在 pdf、图像中显示为块。<br/>设置 DefaultFont，例如 MingLiu 或 MS Gothic 以显示这些字符。<br/>如果不设置该属性，Aspose.Cells 将使用系统默认字体来显示这些 unicode 字符。|
| [check_workbook_default_font](/cells/zh/python-net/aspose.cells/pdfsaveoptions/check_workbook_default_font) |当Excel中的字符是Unicode且未在单元格样式中设置正确的字体时，<br/>它们可能在 pdf、图像中显示为块。<br/>将此设置为 true 以尝试使用工作簿的默认字体首先显示这些字符。|
| [check_font_compatibility](/cells/zh/python-net/aspose.cells/pdfsaveoptions/check_font_compatibility) |指示是否检查文本中每个字符的字体兼容性。|
| [is_font_substitution_char_granularity](/cells/zh/python-net/aspose.cells/pdfsaveoptions/is_font_substitution_char_granularity) |指示当单元格字体不兼容时是否仅替换字符的字体。|
| [one_page_per_sheet](/cells/zh/python-net/aspose.cells/pdfsaveoptions/one_page_per_sheet) |如果 OnePagePerSheet 为 true ，结果中一张纸的所有内容将只输出一页。<br/> pagesetup的纸张大小会失效，pagesetup的其他设置<br/>仍然会生效。|
| [all_columns_in_one_page_per_sheet](/cells/zh/python-net/aspose.cells/pdfsaveoptions/all_columns_in_one_page_per_sheet) |如果 AllColumnsInOnePagePerSheet 为 true ，则一张工作表的所有列内容将仅输出到一页结果。<br/> pagesetup 的纸张大小的宽度将被忽略，pagesetup 的其他设置<br/>仍然会生效。|
| [ignore_error](/cells/zh/python-net/aspose.cells/pdfsaveoptions/ignore_error) |指示是否需要在渲染时隐藏错误。<br/>错误可能是形状、图像、图表渲染等方面的错误。|
| [output_blank_page_when_nothing_to_print](/cells/zh/python-net/aspose.cells/pdfsaveoptions/output_blank_page_when_nothing_to_print) |指示当没有可打印的内容时是否输出空白页。|
| [page_index](/cells/zh/python-net/aspose.cells/pdfsaveoptions/page_index) |获取或设置要保存的第一个页面的从 0 开始的索引。|
| [page_count](/cells/zh/python-net/aspose.cells/pdfsaveoptions/page_count) |获取或设置要保存的页数。|
| [printing_page_type](/cells/zh/python-net/aspose.cells/pdfsaveoptions/printing_page_type) |指示将不打印哪些页面。|
| [gridline_type](/cells/zh/python-net/aspose.cells/pdfsaveoptions/gridline_type) |获取或设置网格线类型。|
| [text_cross_type](/cells/zh/python-net/aspose.cells/pdfsaveoptions/text_cross_type) |获取或设置当文本宽度大于单元格宽度时显示的文本类型。|
| [default_edit_language](/cells/zh/python-net/aspose.cells/pdfsaveoptions/default_edit_language) |获取或设置默认编辑语言。|
| [sheet_set](/cells/zh/python-net/aspose.cells/pdfsaveoptions/sheet_set) |获取或设置要呈现的工作表。默认为工作簿中的所有可见工作表：[SheetSet.visible](/cells/zh/python-net/aspose.cells.rendering/sheetset#visible)。|
| [draw_object_event_handler](/cells/zh/python-net/aspose.cells/pdfsaveoptions/draw_object_event_handler) |实现该接口，在渲染时获取DrawObject和Bound。|
| [page_saving_callback](/cells/zh/python-net/aspose.cells/pdfsaveoptions/page_saving_callback) |控制/指示页面保存过程的进度。|
| [embed_standard_windows_fonts](/cells/zh/python-net/aspose.cells/pdfsaveoptions/embed_standard_windows_fonts) | True 以嵌入 True Type 字体。<br/>仅影响 ASCII 字符 32-127。<br/>字符代码大于 127 的字体总是被嵌入。<br/>始终嵌入 PDF/A-1a、PDF/A-1b 标准的字体。<br/>默认为真。|
| [bookmark](/cells/zh/python-net/aspose.cells/pdfsaveoptions/bookmark) |获取和设置 [PdfBookmarkEntry](/cells/zh/python-net/aspose.cells.rendering/pdfbookmarkentry) 对象。|
| [compliance](/cells/zh/python-net/aspose.cells/pdfsaveoptions/compliance) |工作簿将根据此属性中的 PdfCompliance 转换为 pdf。|
| [security_options](/cells/zh/python-net/aspose.cells/pdfsaveoptions/security_options) |在 xls2pdf 结果中需要安全性时设置此选项。|
| [image_type](/cells/zh/python-net/aspose.cells/pdfsaveoptions/image_type) |表示转换图表和形状时的图像类型。|
| [calculate_formula](/cells/zh/python-net/aspose.cells/pdfsaveoptions/calculate_formula) |指示是否在保存 pdf 文件之前计算公式。|
| [pdf_compression](/cells/zh/python-net/aspose.cells/pdfsaveoptions/pdf_compression) |指明压缩算法|
| [created_time](/cells/zh/python-net/aspose.cells/pdfsaveoptions/created_time) |获取和设置生成pdf文档的时间。|
| [producer](/cells/zh/python-net/aspose.cells/pdfsaveoptions/producer) |获取和设置生成的 pdf 文档的制作者。|
| [optimization_type](/cells/zh/python-net/aspose.cells/pdfsaveoptions/optimization_type) |获取和设置 pdf 优化类型。|
| [custom_properties_export](/cells/zh/python-net/aspose.cells/pdfsaveoptions/custom_properties_export) |获取或设置一个值，该值确定将 [CustomDocumentPropertyCollection](/cells/zh/python-net/aspose.cells.properties/customdocumentpropertycollection) 导出到 PDF 文件的方式。默认值为无。|
| [export_document_structure](/cells/zh/python-net/aspose.cells/pdfsaveoptions/export_document_structure) |指示是否导出文档结构。|
| [emf_render_setting](/cells/zh/python-net/aspose.cells/pdfsaveoptions/emf_render_setting) |渲染 Emf 图元文件的设置。|
| [display_doc_title](/cells/zh/python-net/aspose.cells/pdfsaveoptions/display_doc_title) |指示窗口的标题栏是否应显示文档标题。|
| [font_encoding](/cells/zh/python-net/aspose.cells/pdfsaveoptions/font_encoding) |获取或设置 pdf 中的嵌入字体编码。|


### 方法
|方法|描述|
| :- | :- |
| [set_image_resample(desired_ppi, jpeg_quality)](/cells/zh/python-net/aspose.cells/pdfsaveoptions/set_image_resample/#int-int) |设置重采样图像和 jpeg 质量所需的 PPI（每英寸像素）。<br/>所有图像都将转换为具有指定质量设置的 JPEG，<br/>并且大于指定 PPI（每英寸像素数）的图像将被重新采样。|



### 也可以看看
* 模块 [aspose.cells](..)
* 类 [CustomDocumentPropertyCollection](/cells/zh/python-net/aspose.cells.properties/customdocumentpropertycollection)
* 类 [PaginatedSaveOptions](/cells/zh/python-net/aspose.cells/paginatedsaveoptions)
* 类 [PdfBookmarkEntry](/cells/zh/python-net/aspose.cells.rendering/pdfbookmarkentry)
* 类 [PdfSaveOptions](/cells/zh/python-net/aspose.cells/pdfsaveoptions)
* 类 [SaveOptions](/cells/zh/python-net/aspose.cells/saveoptions)
