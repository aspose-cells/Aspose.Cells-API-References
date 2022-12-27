---
title: HtmlSaveOptions class
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 780
url: /python-net/aspose.cells/htmlsaveoptions/
is_root: false
---

## HtmlSaveOptions class

Represents the options for saving html file.



**Inheritance:** [HtmlSaveOptions](/cells/python-net/aspose.cells/htmlsaveoptions) → 
[SaveOptions](/cells/python-net/aspose.cells/saveoptions)



The HtmlSaveOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [HtmlSaveOptions()](/cells/python-net/aspose.cells/htmlsaveoptions/__init__/#) | Creates options for saving html file. |
| [HtmlSaveOptions(format)](/cells/python-net/aspose.cells/htmlsaveoptions/__init__/#SaveFormat) | Creates options for saving htm file. |


### Properties
| Property | Description |
| :- | :- |
| [save_format](/cells/python-net/aspose.cells/htmlsaveoptions/save_format) | Gets the save file format. |
| [clear_data](/cells/python-net/aspose.cells/htmlsaveoptions/clear_data) | Make the workbook empty after saving the file. |
| [cached_file_folder](/cells/python-net/aspose.cells/htmlsaveoptions/cached_file_folder) | The cached file folder is used to store some large data. |
| [validate_merged_areas](/cells/python-net/aspose.cells/htmlsaveoptions/validate_merged_areas) | Indicates whether validate merged cells before saving the file. |
| [merge_areas](/cells/python-net/aspose.cells/htmlsaveoptions/merge_areas) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [create_directory](/cells/python-net/aspose.cells/htmlsaveoptions/create_directory) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [sort_names](/cells/python-net/aspose.cells/htmlsaveoptions/sort_names) | Indicates whether sorting defined names before saving file. |
| [sort_external_names](/cells/python-net/aspose.cells/htmlsaveoptions/sort_external_names) | Indicates whether sorting external defined names before saving file. |
| [refresh_chart_cache](/cells/python-net/aspose.cells/htmlsaveoptions/refresh_chart_cache) | Indicates whether refreshing chart cache data |
| [warning_callback](/cells/python-net/aspose.cells/htmlsaveoptions/warning_callback) | Gets or sets warning callback. |
| [update_smart_art](/cells/python-net/aspose.cells/htmlsaveoptions/update_smart_art) | Indicates whether updating smart art setting.<br/>The default value is false. |
| [ignore_invisible_shapes](/cells/python-net/aspose.cells/htmlsaveoptions/ignore_invisible_shapes) | Indicate whether exporting those not visible shapes |
| [page_title](/cells/python-net/aspose.cells/htmlsaveoptions/page_title) | The title of the html page.<br/>Only for saving to html stream. |
| [attached_files_directory](/cells/python-net/aspose.cells/htmlsaveoptions/attached_files_directory) | The directory that the attached files will be saved to.<br/>Only for saving to html stream. |
| [attached_files_url_prefix](/cells/python-net/aspose.cells/htmlsaveoptions/attached_files_url_prefix) | Specify the Url prefix of attached files such as image in the html file.<br/>Only for saving to html stream. |
| [default_font_name](/cells/python-net/aspose.cells/htmlsaveoptions/default_font_name) | Specify the default font name for exporting html, the default font will be used  when the font of style is not existing,<br/>If this property is null, Aspose.Cells will use universal font which have the same family with the original font,<br/>the default value is null. |
| [worksheet_scalable](/cells/python-net/aspose.cells/htmlsaveoptions/worksheet_scalable) | Indicates if zooming in or out the html via worksheet zoom level when saving file to html, the default value is false. |
| [is_export_comments](/cells/python-net/aspose.cells/htmlsaveoptions/is_export_comments) | Indicates if exporting comments when saving file to html, the default value is false. |
| [export_comments_type](/cells/python-net/aspose.cells/htmlsaveoptions/export_comments_type) | Represents type of exporting comments to html files. |
| [disable_downlevel_revealed_comments](/cells/python-net/aspose.cells/htmlsaveoptions/disable_downlevel_revealed_comments) | Indicates if disable Downlevel-revealed conditional comments when exporting file to html, the default value is false. |
| [is_exp_image_to_temp_dir](/cells/python-net/aspose.cells/htmlsaveoptions/is_exp_image_to_temp_dir) | Indicates whether exporting image files to temp directory.<br/>Only for saving to html stream. |
| [image_scalable](/cells/python-net/aspose.cells/htmlsaveoptions/image_scalable) | Indicates whether using scalable unit to describe the image width<br/>when using scalable unit to describe the column width.<br/>The default value is true. |
| [width_scalable](/cells/python-net/aspose.cells/htmlsaveoptions/width_scalable) | Indicates whether using scalable unit to describe the column width when exporting file to html.<br/>The default value is false. |
| [export_single_tab](/cells/python-net/aspose.cells/htmlsaveoptions/export_single_tab) | Indicates whether exporting the single tab when the file only has one worksheet.<br/>The default value is false. |
| [export_images_as_base64](/cells/python-net/aspose.cells/htmlsaveoptions/export_images_as_base64) | Specifies whether images are saved in Base64 format to HTML, MHTML or EPUB. |
| [export_active_worksheet_only](/cells/python-net/aspose.cells/htmlsaveoptions/export_active_worksheet_only) | Indicates if exporting the whole workbook to html file. |
| [export_print_area_only](/cells/python-net/aspose.cells/htmlsaveoptions/export_print_area_only) | Indicates if only exporting the print area to html file. The default value is false. |
| [export_area](/cells/python-net/aspose.cells/htmlsaveoptions/export_area) | Gets or Sets the exporting CellArea of current active Worksheet.<br/>If you set this attribute, the print area of current active Worksheet will be omitted.<br/>Only the specified area will be exported when saving the file to html. |
| [parse_html_tag_in_cell](/cells/python-net/aspose.cells/htmlsaveoptions/parse_html_tag_in_cell) | Parse html tag in cell,like ,as cell value,or as html tag,default is true |
| [html_cross_string_type](/cells/python-net/aspose.cells/htmlsaveoptions/html_cross_string_type) | Indicates if a cross-cell string will be displayed in the same way as MS Excel when saving an Excel file in html format.<br/>By default the value is Default, so, for cross-cell strings, there is little difference between the html files created by Aspose.Cells and MS Excel.<br/>But the performance for creating large html files,setting the value to Cross would be several times faster than setting it to Default or Fit2Cell. |
| [hidden_col_display_type](/cells/python-net/aspose.cells/htmlsaveoptions/hidden_col_display_type) | Hidden column(the width of this column is 0) in excel,before save this into html format,<br/>if HtmlHiddenColDisplayType is "Remove",the hidden column would not been output,<br/>if the value is "Hidden", the column would been output,but was hidden,the default value is "Hidden" |
| [hidden_row_display_type](/cells/python-net/aspose.cells/htmlsaveoptions/hidden_row_display_type) | Hidden row(the height of this row is 0) in excel,before save this into html format,<br/>if HtmlHiddenRowDisplayType is "Remove",the hidden row would not been output,<br/>if the value is "Hidden", the row would been output,but was hidden,the default value is "Hidden" |
| [encoding](/cells/python-net/aspose.cells/htmlsaveoptions/encoding) | If not set,use Encoding.UTF8 as default enconding type. |
| [export_object_listener](/cells/python-net/aspose.cells/htmlsaveoptions/export_object_listener) | Gets or sets the ExportObjectListener for exporting objects. |
| [file_path_provider](/cells/python-net/aspose.cells/htmlsaveoptions/file_path_provider) | Gets or sets the IFilePathProvider for exporting Worksheet to html separately. |
| [stream_provider](/cells/python-net/aspose.cells/htmlsaveoptions/stream_provider) | Gets or sets the IStreamProvider for exporting objects. |
| [image_options](/cells/python-net/aspose.cells/htmlsaveoptions/image_options) | Get the ImageOrPrintOptions object before exporting |
| [save_as_single_file](/cells/python-net/aspose.cells/htmlsaveoptions/save_as_single_file) | Indicates whether save the html as single file.<br/>The default value is false. |
| [show_all_sheets](/cells/python-net/aspose.cells/htmlsaveoptions/show_all_sheets) | Indicates whether showing all sheets when saving  as a single html file. |
| [export_page_headers](/cells/python-net/aspose.cells/htmlsaveoptions/export_page_headers) | Indicates whether exporting page headers. |
| [export_page_footers](/cells/python-net/aspose.cells/htmlsaveoptions/export_page_footers) | Indicates whether exporting page headers. |
| [export_hidden_worksheet](/cells/python-net/aspose.cells/htmlsaveoptions/export_hidden_worksheet) | Indicating if exporting the hidden worksheet content.The default value is true. |
| [presentation_preference](/cells/python-net/aspose.cells/htmlsaveoptions/presentation_preference) | Indicating if html or mht file is presentation preference.<br/>The default value is false.<br/>if you want to get more beautiful presentation,please set the value to true. |
| [cell_css_prefix](/cells/python-net/aspose.cells/htmlsaveoptions/cell_css_prefix) | Gets and sets the prefix of the css name,the default value is "". |
| [table_css_id](/cells/python-net/aspose.cells/htmlsaveoptions/table_css_id) | Gets and sets the prefix of the type css name such as tr,col,td and so on, they are contained in the table element <br/>which has the specific TableCssId attribute. The default value is "". |
| [is_full_path_link](/cells/python-net/aspose.cells/htmlsaveoptions/is_full_path_link) | Indicating whether using full path link in sheet00x.htm,filelist.xml and tabstrip.htm.<br/>The default value is false. |
| [export_worksheet_css_separately](/cells/python-net/aspose.cells/htmlsaveoptions/export_worksheet_css_separately) | Indicating whether export the worksheet css separately.The default value is false. |
| [export_similar_border_style](/cells/python-net/aspose.cells/htmlsaveoptions/export_similar_border_style) | Indicating whether exporting the similar border style when the border style is not supported by browsers.<br/>If you want to import the html or mht file to excel, please keep the default value.<br/>The default value is false. |
| [merge_empty_td_forcely](/cells/python-net/aspose.cells/htmlsaveoptions/merge_empty_td_forcely) | Indicates whether merging empty TD element forcedly when exporting file to html. <br/>The size of html file will be reduced significantly after setting value to true. The default value is false. <br/>If you want to import the html file to excel or export perfect grid lines when saving file to html, <br/>please keep the default value. |
| [export_cell_coordinate](/cells/python-net/aspose.cells/htmlsaveoptions/export_cell_coordinate) | Indicates whether exporting excel coordinate of nonblank cells when saving file to html. The default value is false.<br/>If you want to import the output html to excel, please keep the default value. |
| [export_extra_headings](/cells/python-net/aspose.cells/htmlsaveoptions/export_extra_headings) | Indicates whether exporting extra headings when the length of text is longer than max display column.<br/>The default value is false. If you want to import the html file to excel, please keep the default value. |
| [export_headings](/cells/python-net/aspose.cells/htmlsaveoptions/export_headings) | Indicates whether exports sheet's row and column headings when saving to HTML files. |
| [export_row_column_headings](/cells/python-net/aspose.cells/htmlsaveoptions/export_row_column_headings) | Indicates whether exports sheet's row and column headings when saving to HTML files. |
| [export_formula](/cells/python-net/aspose.cells/htmlsaveoptions/export_formula) | Indicates whether exporting formula when saving file to html. The default value is true.<br/>If you want to import the output html to excel, please keep the default value. |
| [add_tooltip_text](/cells/python-net/aspose.cells/htmlsaveoptions/add_tooltip_text) | Indicates whether adding tooltip text when the data can't be fully displayed.<br/>The default value is false. |
| [export_grid_lines](/cells/python-net/aspose.cells/htmlsaveoptions/export_grid_lines) | Indicating whether exporting the gridlines.The default value is false. |
| [export_bogus_row_data](/cells/python-net/aspose.cells/htmlsaveoptions/export_bogus_row_data) | Indicating whether exporting bogus bottom row data. The default value is true.If you want to import the html or mht file<br/>to excel, please keep the default value. |
| [exclude_unused_styles](/cells/python-net/aspose.cells/htmlsaveoptions/exclude_unused_styles) | Indicating whether excludes unused styles.<br/>For the generated html files, excluding unused styles can make the file size smaller<br/>without affecting the visual effects. So the default value of this property is true.<br/>If user needs to keep all styles in the workbook for the generated html(such as the scenario that user<br/>needs to restore the workbook from the generated html later), please set this property as false. |
| [export_document_properties](/cells/python-net/aspose.cells/htmlsaveoptions/export_document_properties) | Indicating whether exporting document properties.The default value is true.If you want to import <br/>the html or mht file to excel, please keep the default value. |
| [export_worksheet_properties](/cells/python-net/aspose.cells/htmlsaveoptions/export_worksheet_properties) | Indicating whether exporting worksheet properties.The default value is true.If you want to import <br/>the html or mht file to excel, please keep the default value. |
| [export_workbook_properties](/cells/python-net/aspose.cells/htmlsaveoptions/export_workbook_properties) | Indicating whether exporting workbook properties.The default value is true.If you want to import <br/>the html or mht file to excel, please keep the default value. |
| [export_frame_scripts_and_properties](/cells/python-net/aspose.cells/htmlsaveoptions/export_frame_scripts_and_properties) | Indicating whether exporting frame scripts and document properties. The default value is true.If you want to import the html or mht file<br/>to excel, please keep the default value. |
| [export_data_options](/cells/python-net/aspose.cells/htmlsaveoptions/export_data_options) | Indicating the rule of exporting html file data.The default value is All. |
| [link_target_type](/cells/python-net/aspose.cells/htmlsaveoptions/link_target_type) | Indicating the type of  target attribute in <a> link,The default value is HtmlLinkTargetType.Parent. |


### See Also

* module [aspose.cells](../)
* class [SaveOptions](/cells/python-net/aspose.cells/saveoptions)
