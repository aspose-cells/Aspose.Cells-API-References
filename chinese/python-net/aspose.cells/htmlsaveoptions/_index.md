---
title: HtmlSaveOptions类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 780
url: /zh/python-net/aspose.cells/htmlsaveoptions/
is_root: false
---
## HtmlSaveOptions类
表示保存 html 文件的选项。



**继承：** [HtmlSaveOptions](/cells/python-net/aspose.cells/htmlsaveoptions) → 
[SaveOptions](/cells/zh/python-net/aspose.cells/saveoptions)



HtmlSaveOptions 类型公开了以下成员：

### 构造器
|构造器|描述|
| :- | :- |
| [HtmlSaveOptions()](/cells/zh/python-net/aspose.cells/htmlsaveoptions/__init__/#) |创建用于保存 html 文件的选项。|
| [HtmlSaveOptions(format)](/cells/zh/python-net/aspose.cells/htmlsaveoptions/__init__/#SaveFormat) |创建用于保存 htm 文件的选项。|


### 特性
|属性|描述|
| :- | :- |
| [save_format](/cells/zh/python-net/aspose.cells/htmlsaveoptions/save_format) |获取保存文件格式。|
| [clear_data](/cells/zh/python-net/aspose.cells/htmlsaveoptions/clear_data) |保存文件后将工作簿清空。|
| [cached_file_folder](/cells/zh/python-net/aspose.cells/htmlsaveoptions/cached_file_folder) |缓存文件夹用于存储一些大数据。|
| [validate_merged_areas](/cells/zh/python-net/aspose.cells/htmlsaveoptions/validate_merged_areas) |指示是否在保存文件之前验证合并的单元格。|
| [merge_areas](/cells/zh/python-net/aspose.cells/htmlsaveoptions/merge_areas) |指示是否在保存文件之前合并条件格式和验证区域。|
| [create_directory](/cells/zh/python-net/aspose.cells/htmlsaveoptions/create_directory) |如果为 true 并且目录不存在，则在保存文件之前会自动创建目录。|
| [sort_names](/cells/zh/python-net/aspose.cells/htmlsaveoptions/sort_names) |指示是否在保存文件之前对定义的名称进行排序。|
| [sort_external_names](/cells/zh/python-net/aspose.cells/htmlsaveoptions/sort_external_names) |指示是否在保存文件之前对外部定义的名称进行排序。|
| [refresh_chart_cache](/cells/zh/python-net/aspose.cells/htmlsaveoptions/refresh_chart_cache) |指示是否刷新图表缓存数据|
| [warning_callback](/cells/zh/python-net/aspose.cells/htmlsaveoptions/warning_callback) |获取或设置警告回调。|
| [update_smart_art](/cells/zh/python-net/aspose.cells/htmlsaveoptions/update_smart_art) |指示是否更新智能艺术设置。<br/>默认值为假。|
| [ignore_invisible_shapes](/cells/zh/python-net/aspose.cells/htmlsaveoptions/ignore_invisible_shapes) |指示是否导出那些不可见的形状|
| [page_title](/cells/zh/python-net/aspose.cells/htmlsaveoptions/page_title) |html 页面的标题。<br/>仅用于保存到 html 流。|
| [attached_files_directory](/cells/zh/python-net/aspose.cells/htmlsaveoptions/attached_files_directory) |附加文件将保存到的目录。<br/>仅用于保存到 html 流。|
| [attached_files_url_prefix](/cells/zh/python-net/aspose.cells/htmlsaveoptions/attached_files_url_prefix) |指定附加文件的 Url 前缀，例如 html 文件中的图像。<br/>仅用于保存到 html 流。|
| [default_font_name](/cells/zh/python-net/aspose.cells/htmlsaveoptions/default_font_name) |指定导出html的默认字体名称，当style字体不存在时使用默认字体，<br/>如果此属性为空，Aspose.Cells 将使用与原始字体同族的通用字体，<br/>默认值为空。|
| [worksheet_scalable](/cells/zh/python-net/aspose.cells/htmlsaveoptions/worksheet_scalable) |指示在将文件保存为 html 时是否通过工作表缩放级别放大或缩小 html，默认值为 false。|
| [is_export_comments](/cells/zh/python-net/aspose.cells/htmlsaveoptions/is_export_comments) |表示保存为html时是否导出注释，默认为false。|
| [export_comments_type](/cells/zh/python-net/aspose.cells/htmlsaveoptions/export_comments_type) |表示将评论导出到 html 文件的类型。|
| [disable_downlevel_revealed_comments](/cells/zh/python-net/aspose.cells/htmlsaveoptions/disable_downlevel_revealed_comments) |指示在将文件导出为 html 时是否禁用 Downlevel-revealed 条件注释，默认值为 false。|
| [is_exp_image_to_temp_dir](/cells/zh/python-net/aspose.cells/htmlsaveoptions/is_exp_image_to_temp_dir) |指示是否将图像文件导出到临时目录。<br/>仅用于保存到 html 流。|
| [image_scalable](/cells/zh/python-net/aspose.cells/htmlsaveoptions/image_scalable) |指示是否使用可伸缩单位来描述图像宽度<br/>当使用可伸缩单位来描述列宽时。<br/>默认值是true。|
| [width_scalable](/cells/zh/python-net/aspose.cells/htmlsaveoptions/width_scalable) |指示在将文件导出为 html 时是否使用可伸缩单位来描述列宽。<br/>默认值为假。|
| [export_single_tab](/cells/zh/python-net/aspose.cells/htmlsaveoptions/export_single_tab) |当文件只有一张工作表时是否导出单个标签。<br/>默认值为假。|
| [export_images_as_base64](/cells/zh/python-net/aspose.cells/htmlsaveoptions/export_images_as_base64) |指定图像是否以 Base64 格式保存到 HTML、MHTML 或 EPUB。|
| [export_active_worksheet_only](/cells/zh/python-net/aspose.cells/htmlsaveoptions/export_active_worksheet_only) |指示是否将整个工作簿导出到 html 文件。|
| [export_print_area_only](/cells/zh/python-net/aspose.cells/htmlsaveoptions/export_print_area_only) |表示是否只将打印区域导出到html文件。默认值为假。|
| [export_area](/cells/zh/python-net/aspose.cells/htmlsaveoptions/export_area) |获取或设置当前活动工作表的导出单元格区域。<br/>如果设置该属性，则当前活动工作表的打印区域将被忽略。<br/>将文件保存为 html 时，只会导出指定区域。|
| [parse_html_tag_in_cell](/cells/zh/python-net/aspose.cells/htmlsaveoptions/parse_html_tag_in_cell) |解析单元格中的 html 标签，如，作为单元格值，或作为 html 标签，默认为 true|
| [html_cross_string_type](/cells/zh/python-net/aspose.cells/htmlsaveoptions/html_cross_string_type) |指示在以 html 格式保存 Excel 文件时，是否以与 MS Excel 相同的方式显示跨单元格字符串。<br/>默认情况下，该值为 Default，因此，对于跨单元格字符串，Aspose.Cells 和 MS Excel 创建的 html 文件之间几乎没有区别。<br/>但是创建大型 html 文件的性能，将值设置为 Cross 将比将其设置为 Default 或 Fit2Cell 快几倍。|
| [hidden_col_display_type](/cells/zh/python-net/aspose.cells/htmlsaveoptions/hidden_col_display_type) |excel中的隐藏列（该列的宽度为0），在保存为html格式之前，<br/>如果 HtmlHiddenColDisplayType 为“Remove”，则隐藏列不会输出，<br/>如果值为“Hidden”，该列将被输出，但被隐藏，默认值为“Hidden”|
| [hidden_row_display_type](/cells/zh/python-net/aspose.cells/htmlsaveoptions/hidden_row_display_type) | excel隐藏行（行高为0），保存成html格式前，<br/>如果 HtmlHiddenRowDisplayType 为“Remove”，则隐藏行不会输出，<br/>如果值为“Hidden”，该行将被输出，但被隐藏，默认值为“Hidden”|
| [encoding](/cells/zh/python-net/aspose.cells/htmlsaveoptions/encoding) |如果未设置，则使用 Encoding.UTF8 作为默认编码类型。|
| [export_object_listener](/cells/zh/python-net/aspose.cells/htmlsaveoptions/export_object_listener) |获取或设置用于导出对象的 ExportObjectListener。|
| [file_path_provider](/cells/zh/python-net/aspose.cells/htmlsaveoptions/file_path_provider) |单独获取或设置用于将Worksheet导出为html的IFilePathProvider。|
| [stream_provider](/cells/zh/python-net/aspose.cells/htmlsaveoptions/stream_provider) |获取或设置用于导出对象的 IStreamProvider。|
| [image_options](/cells/zh/python-net/aspose.cells/htmlsaveoptions/image_options) |导出前获取 ImageOrPrintOptions 对象|
| [save_as_single_file](/cells/zh/python-net/aspose.cells/htmlsaveoptions/save_as_single_file) |指示是否将 html 保存为单个文件。<br/>默认值为假。|
| [show_all_sheets](/cells/zh/python-net/aspose.cells/htmlsaveoptions/show_all_sheets) |指示在保存为单个 html 文件时是否显示所有工作表。|
| [export_page_headers](/cells/zh/python-net/aspose.cells/htmlsaveoptions/export_page_headers) |是否导出页眉。|
| [export_page_footers](/cells/zh/python-net/aspose.cells/htmlsaveoptions/export_page_footers) |是否导出页眉。|
| [export_hidden_worksheet](/cells/zh/python-net/aspose.cells/htmlsaveoptions/export_hidden_worksheet) |表示是否导出隐藏的工作表内容。默认值为true。|
| [presentation_preference](/cells/zh/python-net/aspose.cells/htmlsaveoptions/presentation_preference) |指示 html 或 mht 文件是否是演示文稿首选项。<br/>默认值为假。<br/>如果你想获得更漂亮的呈现，请将值设置为 true。|
| [cell_css_prefix](/cells/zh/python-net/aspose.cells/htmlsaveoptions/cell_css_prefix) |获取和设置css名称的前缀，默认值为""。|
| [table_css_id](/cells/zh/python-net/aspose.cells/htmlsaveoptions/table_css_id) |获取和设置类型css名称的前缀，如tr,col,td等，它们包含在table元素中<br/>它具有特定的 TableCssId 属性。默认值为“”。|
| [is_full_path_link](/cells/zh/python-net/aspose.cells/htmlsaveoptions/is_full_path_link) |在 sheet00x.htm、filelist.xml 和 tabstrip.htm 中指明是否使用全路径链接。<br/>默认值为假。|
| [export_worksheet_css_separately](/cells/zh/python-net/aspose.cells/htmlsaveoptions/export_worksheet_css_separately) |表示是否单独导出工作表css。默认值为false。|
| [export_similar_border_style](/cells/zh/python-net/aspose.cells/htmlsaveoptions/export_similar_border_style) |指示当浏览器不支持边框样式时是否导出相似的边框样式。<br/>如果要将 html 或 mht 文件导入到 excel，请保持默认值。<br/>默认值为假。|
| [merge_empty_td_forcely](/cells/zh/python-net/aspose.cells/htmlsaveoptions/merge_empty_td_forcely) |指示在将文件导出为 html 时是否强制合并空 TD 元素。<br/>将值设置为true后，html文件的大小将显着减小。默认值为假。<br/>如果你想将html文件导入excel或者在保存文件到html时导出完美的网格线，<br/>请保持默认值。|
| [export_cell_coordinate](/cells/zh/python-net/aspose.cells/htmlsaveoptions/export_cell_coordinate) |指示在将文件保存为 html 时是否导出非空白单元格的 excel 坐标。默认值为假。<br/>如果要将输出的html导入到excel中，请保持默认值。|
| [export_extra_headings](/cells/zh/python-net/aspose.cells/htmlsaveoptions/export_extra_headings) |指示当文本长度超过最大显示列时是否导出额外的标题。<br/>默认值为假。如果要将html文件导入excel，请保持默认值。|
| [export_headings](/cells/zh/python-net/aspose.cells/htmlsaveoptions/export_headings) |指示在保存到 HTML 文件时是否导出工作表的行和列标题。|
| [export_row_column_headings](/cells/zh/python-net/aspose.cells/htmlsaveoptions/export_row_column_headings) |指示在保存到 HTML 文件时是否导出工作表的行和列标题。|
| [export_formula](/cells/zh/python-net/aspose.cells/htmlsaveoptions/export_formula) |保存文件为html时是否导出公式。默认值是true。<br/>如果要将输出的html导入到excel中，请保持默认值。|
| [add_tooltip_text](/cells/zh/python-net/aspose.cells/htmlsaveoptions/add_tooltip_text) |表示当数据无法完全显示时是否添加工具提示文本。<br/>默认值为假。|
| [export_grid_lines](/cells/zh/python-net/aspose.cells/htmlsaveoptions/export_grid_lines) |是否导出网格线，默认为false。|
| [export_bogus_row_data](/cells/zh/python-net/aspose.cells/htmlsaveoptions/export_bogus_row_data) |提示是否导出伪造的底行数据。默认值为true。如果要导入html或mht文件<br/>excel，请保持默认值。|
| [exclude_unused_styles](/cells/zh/python-net/aspose.cells/htmlsaveoptions/exclude_unused_styles) |指示是否排除未使用的样式。<br/>对于生成的html文件，排除不用的样式可以使文件体积更小<br/>在不影响视觉效果的情况下。所以这个属性的默认值为真。<br/>如果用户需要为生成的 html 保留工作簿中的所有样式（例如用户的场景<br/>稍后需要从生成的 html 中恢复工作簿），请将此属性设置为 false。|
| [export_document_properties](/cells/zh/python-net/aspose.cells/htmlsaveoptions/export_document_properties) |表示是否导出文档属性。默认值为true。如果要导入<br/>html或mht文件转excel，请保持默认值。|
| [export_worksheet_properties](/cells/zh/python-net/aspose.cells/htmlsaveoptions/export_worksheet_properties) |表示是否导出工作表属性。默认值为true。如果要导入<br/>html或mht文件转excel，请保持默认值。|
| [export_workbook_properties](/cells/zh/python-net/aspose.cells/htmlsaveoptions/export_workbook_properties) |表示是否导出工作簿属性。默认值为true。如果要导入<br/>html或mht文件转excel，请保持默认值。|
| [export_frame_scripts_and_properties](/cells/zh/python-net/aspose.cells/htmlsaveoptions/export_frame_scripts_and_properties) |指示是否导出框架脚本和文档属性。默认值为true。如果要导入html或mht文件<br/>excel，请保持默认值。|
| [export_data_options](/cells/zh/python-net/aspose.cells/htmlsaveoptions/export_data_options) |表示导出html文件数据的规则，默认为全部。|
| [link_target_type](/cells/zh/python-net/aspose.cells/htmlsaveoptions/link_target_type) |指示目标属性的类型<a>link，默认值为HtmlLinkTargetType.Parent。|



### 也可以看看
* 模块 [aspose.cells](..)
* 类 [HtmlSaveOptions](/cells/zh/python-net/aspose.cells/htmlsaveoptions)
* 类 [SaveOptions](/cells/zh/python-net/aspose.cells/saveoptions)
