---
title: PptxSaveOptions类
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 1190
url: /zh/python-net/aspose.cells/pptxsaveoptions/
is_root: false
---
## PptxSaveOptions类
表示 pptx 保存选项。



**继承：** [PptxSaveOptions](/cells/python-net/aspose.cells/pptxsaveoptions) → 
[PaginatedSaveOptions](/cells/python-net/aspose.cells/paginatedsaveoptions) → 
[SaveOptions](/cells/zh/python-net/aspose.cells/saveoptions)



PptxSaveOptions 类型公开了以下成员：

### 构造器
|构造器|描述|
| :- | :- |
| [PptxSaveOptions()](/cells/zh/python-net/aspose.cells/pptxsaveoptions/__init__/#) |表示 pptx 保存选项。|
| [PptxSaveOptions(save_as_image)](/cells/zh/python-net/aspose.cells/pptxsaveoptions/__init__/#bool) |表示保存 .pptx 文件的选项。|


### 特性
|属性|描述|
| :- | :- |
| [save_format](/cells/zh/python-net/aspose.cells/pptxsaveoptions/save_format) |获取保存文件格式。|
| [clear_data](/cells/zh/python-net/aspose.cells/pptxsaveoptions/clear_data) |保存文件后将工作簿清空。|
| [cached_file_folder](/cells/zh/python-net/aspose.cells/pptxsaveoptions/cached_file_folder) |缓存文件夹用于存储一些大数据。|
| [validate_merged_areas](/cells/zh/python-net/aspose.cells/pptxsaveoptions/validate_merged_areas) |指示是否在保存文件之前验证合并的单元格。|
| [merge_areas](/cells/zh/python-net/aspose.cells/pptxsaveoptions/merge_areas) |指示是否在保存文件之前合并条件格式和验证区域。|
| [create_directory](/cells/zh/python-net/aspose.cells/pptxsaveoptions/create_directory) |如果为 true 并且目录不存在，则在保存文件之前会自动创建目录。|
| [sort_names](/cells/zh/python-net/aspose.cells/pptxsaveoptions/sort_names) |指示是否在保存文件之前对定义的名称进行排序。|
| [sort_external_names](/cells/zh/python-net/aspose.cells/pptxsaveoptions/sort_external_names) |指示是否在保存文件之前对外部定义的名称进行排序。|
| [refresh_chart_cache](/cells/zh/python-net/aspose.cells/pptxsaveoptions/refresh_chart_cache) |指示是否刷新图表缓存数据|
| [warning_callback](/cells/zh/python-net/aspose.cells/pptxsaveoptions/warning_callback) |获取或设置警告回调。|
| [update_smart_art](/cells/zh/python-net/aspose.cells/pptxsaveoptions/update_smart_art) |指示是否更新智能艺术设置。<br/>默认值为假。|
| [default_font](/cells/zh/python-net/aspose.cells/pptxsaveoptions/default_font) |当Excel中的字符是Unicode且未在单元格样式中设置正确的字体时，<br/>它们可能在 pdf、图像中显示为块。<br/>设置 DefaultFont，例如 MingLiu 或 MS Gothic 以显示这些字符。<br/>如果不设置该属性，Aspose.Cells 将使用系统默认字体来显示这些 unicode 字符。|
| [check_workbook_default_font](/cells/zh/python-net/aspose.cells/pptxsaveoptions/check_workbook_default_font) |当Excel中的字符是Unicode且未在单元格样式中设置正确的字体时，<br/>它们可能在 pdf、图像中显示为块。<br/>将此设置为 true 以尝试使用工作簿的默认字体首先显示这些字符。|
| [check_font_compatibility](/cells/zh/python-net/aspose.cells/pptxsaveoptions/check_font_compatibility) |指示是否检查文本中每个字符的字体兼容性。|
| [is_font_substitution_char_granularity](/cells/zh/python-net/aspose.cells/pptxsaveoptions/is_font_substitution_char_granularity) |指示是否仅在单元格字体不兼容时替换字符的字体。|
| [one_page_per_sheet](/cells/zh/python-net/aspose.cells/pptxsaveoptions/one_page_per_sheet) |如果 OnePagePerSheet 为 true ，结果中一张纸的所有内容将只输出一页。<br/> pagesetup的纸张大小会失效，pagesetup的其他设置<br/>仍然会生效。|
| [all_columns_in_one_page_per_sheet](/cells/zh/python-net/aspose.cells/pptxsaveoptions/all_columns_in_one_page_per_sheet) |如果 AllColumnsInOnePagePerSheet 为 true ，则一张工作表的所有列内容将仅输出到一页结果。<br/> pagesetup 的纸张大小的宽度将被忽略，pagesetup 的其他设置<br/>仍然会生效。|
| [ignore_error](/cells/zh/python-net/aspose.cells/pptxsaveoptions/ignore_error) |指示是否需要在渲染时隐藏错误。<br/>错误可能是形状、图像、图表渲染等方面的错误。|
| [output_blank_page_when_nothing_to_print](/cells/zh/python-net/aspose.cells/pptxsaveoptions/output_blank_page_when_nothing_to_print) |指示当没有可打印的内容时是否输出空白页。|
| [page_index](/cells/zh/python-net/aspose.cells/pptxsaveoptions/page_index) |获取或设置要保存的第一个页面的从 0 开始的索引。|
| [page_count](/cells/zh/python-net/aspose.cells/pptxsaveoptions/page_count) |获取或设置要保存的页数。|
| [printing_page_type](/cells/zh/python-net/aspose.cells/pptxsaveoptions/printing_page_type) |指示将不打印哪些页面。|
| [gridline_type](/cells/zh/python-net/aspose.cells/pptxsaveoptions/gridline_type) |获取或设置网格线类型。|
| [text_cross_type](/cells/zh/python-net/aspose.cells/pptxsaveoptions/text_cross_type) |获取或设置当文本宽度大于单元格宽度时显示的文本类型。|
| [default_edit_language](/cells/zh/python-net/aspose.cells/pptxsaveoptions/default_edit_language) |获取或设置默认编辑语言。|
| [sheet_set](/cells/zh/python-net/aspose.cells/pptxsaveoptions/sheet_set) |获取或设置要呈现的工作表。默认为工作簿中的所有可见工作表：[SheetSet.visible](/cells/zh/python-net/aspose.cells.rendering/sheetset#visible)。|
| [draw_object_event_handler](/cells/zh/python-net/aspose.cells/pptxsaveoptions/draw_object_event_handler) |实现该接口，在渲染时获取DrawObject和Bound。|
| [page_saving_callback](/cells/zh/python-net/aspose.cells/pptxsaveoptions/page_saving_callback) |控制/指示页面保存过程的进度。|



### 也可以看看
* 模块 [aspose.cells](..)
* 类 [PaginatedSaveOptions](/cells/zh/python-net/aspose.cells/paginatedsaveoptions)
* 类 [PptxSaveOptions](/cells/zh/python-net/aspose.cells/pptxsaveoptions)
* 类 [SaveOptions](/cells/zh/python-net/aspose.cells/saveoptions)
