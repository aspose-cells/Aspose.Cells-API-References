##HtmlSaveOptions class
## HtmlSaveOptions class
Represents the options for saving html file.
**Inheritance:** [`HtmlSaveOptions`](/cells/python-net/aspose.cells/htmlsaveoptions) →
[`SaveOptions`](/cells/python-net/aspose.cells/saveoptions)
The HtmlSaveOptions type exposes the following members:
### Constructors
| Constructor | Description |
| :- | :- |
| [`__init__(self)`](/cells/python-net/aspose.cells/htmlsaveoptions/__init__/#) | Creates options for saving html file. |
| [`__init__(self, save_format)`](/cells/python-net/aspose.cells/htmlsaveoptions/__init__/#aspose.cells.saveformat) | Creates options for saving htm file. |
### Properties
| Property | Description |
| :- | :- |
| [save_format](/cells/python-net/aspose.cells/htmlsaveoptions/save_format) | Gets the save file format. |
| [clear_data](/cells/python-net/aspose.cells/htmlsaveoptions/clear_data) | Make the workbook empty after saving the file. |
| [cached_file_folder](/cells/python-net/aspose.cells/htmlsaveoptions/cached_file_folder) | The folder for temporary files that may be used as data cache. |
| [validate_merged_areas](/cells/python-net/aspose.cells/htmlsaveoptions/validate_merged_areas) | Indicates whether validate merged cells before saving the file. |
| [merge_areas](/cells/python-net/aspose.cells/htmlsaveoptions/merge_areas) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [create_directory](/cells/python-net/aspose.cells/htmlsaveoptions/create_directory) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [sort_names](/cells/python-net/aspose.cells/htmlsaveoptions/sort_names) | Indicates whether sorting defined names before saving file. |
| [sort_external_names](/cells/python-net/aspose.cells/htmlsaveoptions/sort_external_names) | Indicates whether sorting external defined names before saving file. |
| [refresh_chart_cache](/cells/python-net/aspose.cells/htmlsaveoptions/refresh_chart_cache) | Indicates whether refreshing chart cache data |
| [warning_callback](/cells/python-net/aspose.cells/htmlsaveoptions/warning_callback) | Gets or sets warning callback. |
| [check_excel_restriction](/cells/python-net/aspose.cells/htmlsaveoptions/check_excel_restriction) | Whether check restriction of excel file when user modify cells related objects.
| [update_smart_art](/cells/python-net/aspose.cells/htmlsaveoptions/update_smart_art) | Indicates whether updating smart art setting.
| [encrypt_document_properties](/cells/python-net/aspose.cells/htmlsaveoptions/encrypt_document_properties) | Indicates whether encrypt document properties when saving as .xls file.
| [ignore_invisible_shapes](/cells/python-net/aspose.cells/htmlsaveoptions/ignore_invisible_shapes) | Indicate whether exporting those not visible shapes |
| [page_title](/cells/python-net/aspose.cells/htmlsaveoptions/page_title) | The title of the html page.
| [attached_files_directory](/cells/python-net/aspose.cells/htmlsaveoptions/attached_files_directory) | The directory that the attached files will be saved to.
| [attached_files_url_prefix](/cells/python-net/aspose.cells/htmlsaveoptions/attached_files_url_prefix) | Specify the Url prefix of attached files such as image in the html file.
| [default_font_name](/cells/python-net/aspose.cells/htmlsaveoptions/default_font_name) | Specify the default font name for exporting html, the default font will be used  when the font of style is not existing,
| [add_generic_font](/cells/python-net/aspose.cells/htmlsaveoptions/add_generic_font) | Indicates whether to add a generic font to CSS font-family.
| [worksheet_scalable](/cells/python-net/aspose.cells/htmlsaveoptions/worksheet_scalable) | Indicates if zooming in or out the html via worksheet zoom level when saving file to html, the default value is false. |
| [is_export_comments](/cells/python-net/aspose.cells/htmlsaveoptions/is_export_comments) | Indicates if exporting comments when saving file to html, the default value is false. |
| [export_comments_type](/cells/python-net/aspose.cells/htmlsaveoptions/export_comments_type) | Represents type of exporting comments to html files. |
| [disable_downlevel_revealed_comments](/cells/python-net/aspose.cells/htmlsaveoptions/disable_downlevel_revealed_comments) | Indicates if disable Downlevel-revealed conditional comments when exporting file to html, the default value is false. |
| [is_exp_image_to_temp_dir](/cells/python-net/aspose.cells/htmlsaveoptions/is_exp_image_to_temp_dir) | Indicates whether exporting image files to temp directory.
| [image_scalable](/cells/python-net/aspose.cells/htmlsaveoptions/image_scalable) | Indicates whether using scalable unit to describe the image width
| [width_scalable](/cells/python-net/aspose.cells/htmlsaveoptions/width_scalable) | Indicates whether exporting column width in unit of scale to html.
| [export_single_tab](/cells/python-net/aspose.cells/htmlsaveoptions/export_single_tab) | Indicates whether exporting the single tab when the file only has one worksheet.
| [export_images_as_base64](/cells/python-net/aspose.cells/htmlsaveoptions/export_images_as_base64) | Specifies whether images are saved in Base64 format to HTML, MHTML or EPUB. |
| [export_active_worksheet_only](/cells/python-net/aspose.cells/htmlsaveoptions/export_active_worksheet_only) | Indicates if only exporting the active worksheet to html file.
| [export_print_area_only](/cells/python-net/aspose.cells/htmlsaveoptions/export_print_area_only) | Indicates if only exporting the print area to html file. The default value is false. |
| [export_area](/cells/python-net/aspose.cells/htmlsaveoptions/export_area) | Gets or Sets the exporting CellArea of current active Worksheet.
| [parse_html_tag_in_cell](/cells/python-net/aspose.cells/htmlsaveoptions/parse_html_tag_in_cell) | Indicates whether html tag(such as `<div></div>`) in cell should be parsed as cell value or preserved as it is.
| [html_cross_string_type](/cells/python-net/aspose.cells/htmlsaveoptions/html_cross_string_type) | Indicates if a cross-cell string will be displayed in the same way as MS Excel when saving an Excel file in html format.
| [hidden_col_display_type](/cells/python-net/aspose.cells/htmlsaveoptions/hidden_col_display_type) | Hidden column(the width of this column is 0) in excel,before save this into html format,
| [hidden_row_display_type](/cells/python-net/aspose.cells/htmlsaveoptions/hidden_row_display_type) | Hidden row(the height of this row is 0) in excel,before save this into html format,
| [encoding](/cells/python-net/aspose.cells/htmlsaveoptions/encoding) | If not set,use Encoding.UTF8 as default enconding type. |
| [export_object_listener](/cells/python-net/aspose.cells/htmlsaveoptions/export_object_listener) | Gets or sets the ExportObjectListener for exporting objects. |
| [file_path_provider](/cells/python-net/aspose.cells/htmlsaveoptions/file_path_provider) | Gets or sets the IFilePathProvider for exporting Worksheet to html separately. |
| [stream_provider](/cells/python-net/aspose.cells/htmlsaveoptions/stream_provider) | Gets or sets the IStreamProvider for exporting objects. |
| [image_options](/cells/python-net/aspose.cells/htmlsaveoptions/image_options) | Get the ImageOrPrintOptions object before exporting |
| [save_as_single_file](/cells/python-net/aspose.cells/htmlsaveoptions/save_as_single_file) | Indicates whether save the html as single file.
| [show_all_sheets](/cells/python-net/aspose.cells/htmlsaveoptions/show_all_sheets) | Indicates whether showing all sheets when saving  as a single html file. |
| [export_page_headers](/cells/python-net/aspose.cells/htmlsaveoptions/export_page_headers) | Indicates whether exporting page headers. |
| [export_page_footers](/cells/python-net/aspose.cells/htmlsaveoptions/export_page_footers) | Indicates whether exporting page headers. |
| [export_hidden_worksheet](/cells/python-net/aspose.cells/htmlsaveoptions/export_hidden_worksheet) | Indicating if exporting the hidden worksheet content.The default value is true. |
| [presentation_preference](/cells/python-net/aspose.cells/htmlsaveoptions/presentation_preference) | Indicating if html or mht file is presentation preference.
| [cell_css_prefix](/cells/python-net/aspose.cells/htmlsaveoptions/cell_css_prefix) | Gets and sets the prefix of the css name,the default value is "". |
| [table_css_id](/cells/python-net/aspose.cells/htmlsaveoptions/table_css_id) | Gets and sets the prefix of the type css name such as tr,col,td and so on, they are contained in the table element
| [is_full_path_link](/cells/python-net/aspose.cells/htmlsaveoptions/is_full_path_link) | Indicating whether using full path link in sheet00x.htm,filelist.xml and tabstrip.htm.
| [export_worksheet_css_separately](/cells/python-net/aspose.cells/htmlsaveoptions/export_worksheet_css_separately) | Indicating whether export the worksheet css separately.The default value is false. |
| [export_similar_border_style](/cells/python-net/aspose.cells/htmlsaveoptions/export_similar_border_style) | Indicating whether exporting the similar border style when the border style is not supported by browsers.
| [merge_empty_td_forcely](/cells/python-net/aspose.cells/htmlsaveoptions/merge_empty_td_forcely) | Indicates whether merging empty TD element forcedly when exporting file to html.
| [merge_empty_td_type](/cells/python-net/aspose.cells/htmlsaveoptions/merge_empty_td_type) | The option to merge contiguous empty cells(empty td elements)
| [export_cell_coordinate](/cells/python-net/aspose.cells/htmlsaveoptions/export_cell_coordinate) | Indicates whether exporting excel coordinate of nonblank cells when saving file to html. The default value is false.
| [export_extra_headings](/cells/python-net/aspose.cells/htmlsaveoptions/export_extra_headings) | Indicates whether exporting extra headings when the length of text is longer than max display column.
| [export_headings](/cells/python-net/aspose.cells/htmlsaveoptions/export_headings) | Indicates whether exports sheet's row and column headings when saving to HTML files. |
| [export_row_column_headings](/cells/python-net/aspose.cells/htmlsaveoptions/export_row_column_headings) | Indicates whether exports sheet's row and column headings when saving to HTML files. |
| [export_formula](/cells/python-net/aspose.cells/htmlsaveoptions/export_formula) | Indicates whether exporting formula when saving file to html. The default value is true.
| [add_tooltip_text](/cells/python-net/aspose.cells/htmlsaveoptions/add_tooltip_text) | Indicates whether adding tooltip text when the data can't be fully displayed.
| [export_grid_lines](/cells/python-net/aspose.cells/htmlsaveoptions/export_grid_lines) | Indicating whether exporting the gridlines.The default value is false. |
| [export_bogus_row_data](/cells/python-net/aspose.cells/htmlsaveoptions/export_bogus_row_data) | Indicating whether exporting bogus bottom row data. The default value is true.If you want to import the html or mht file
| [exclude_unused_styles](/cells/python-net/aspose.cells/htmlsaveoptions/exclude_unused_styles) | Indicating whether excludes unused styles.
| [export_document_properties](/cells/python-net/aspose.cells/htmlsaveoptions/export_document_properties) | Indicating whether exporting document properties.The default value is true.If you want to import
| [export_worksheet_properties](/cells/python-net/aspose.cells/htmlsaveoptions/export_worksheet_properties) | Indicating whether exporting worksheet properties.The default value is true.If you want to import
| [export_workbook_properties](/cells/python-net/aspose.cells/htmlsaveoptions/export_workbook_properties) | Indicating whether exporting workbook properties.The default value is true.If you want to import
| [export_frame_scripts_and_properties](/cells/python-net/aspose.cells/htmlsaveoptions/export_frame_scripts_and_properties) | Indicating whether exporting frame scripts and document properties. The default value is true.If you want to import the html or mht file
| [export_data_options](/cells/python-net/aspose.cells/htmlsaveoptions/export_data_options) | Indicating the rule of exporting html file data.The default value is All. |
| [link_target_type](/cells/python-net/aspose.cells/htmlsaveoptions/link_target_type) | Indicating the type of target attribute in `<a>` link. The default value is HtmlLinkTargetType.Parent. |
| [is_ie_compatible](/cells/python-net/aspose.cells/htmlsaveoptions/is_ie_compatible) | Indicating whether the output HTML is compatible with IE browser.
| [format_data_ignore_column_width](/cells/python-net/aspose.cells/htmlsaveoptions/format_data_ignore_column_width) | Indicating whether show the whole formatted data of cell when overflowing the column.
| [calculate_formula](/cells/python-net/aspose.cells/htmlsaveoptions/calculate_formula) | Indicates whether to calculate formulas before saving html file. |
| [is_js_browser_compatible](/cells/python-net/aspose.cells/htmlsaveoptions/is_js_browser_compatible) | Indicates whether JavaScript is compatible with browsers that do not support JavaScript.
| [is_mobile_compatible](/cells/python-net/aspose.cells/htmlsaveoptions/is_mobile_compatible) | Indicates whether the output HTML is compatible with mobile devices.
| [css_styles](/cells/python-net/aspose.cells/htmlsaveoptions/css_styles) | Gets or sets the additional css styles for the formatter.
| [hide_overflow_wrapped_text](/cells/python-net/aspose.cells/htmlsaveoptions/hide_overflow_wrapped_text) | Indicates whether to hide overflow text when the cell format is set to wrap text.
| [is_border_collapsed](/cells/python-net/aspose.cells/htmlsaveoptions/is_border_collapsed) | Indicates whether the table borders are collapsed.
| [encode_entity_as_code](/cells/python-net/aspose.cells/htmlsaveoptions/encode_entity_as_code) | Indicates whether the html character entities are replaced with decimal code.
| [office_math_output_mode](/cells/python-net/aspose.cells/htmlsaveoptions/office_math_output_mode) | Indicates how export OfficeMath objects to HTML, Default value is Image. |
| [cell_name_attribute](/cells/python-net/aspose.cells/htmlsaveoptions/cell_name_attribute) | Specifies the attribute that indicates the CellName to be written.
| [disable_css](/cells/python-net/aspose.cells/htmlsaveoptions/disable_css) | Indicates whether only inline styles are applied, without relying on CSS.
| [enable_css_custom_properties](/cells/python-net/aspose.cells/htmlsaveoptions/enable_css_custom_properties) | Optimize the output of html by using CSS custom properties. For example, for the scenario that there are multiple occurences for one base64 image, with custom property the image data only needs to be saved once so the performance of the resultant html can be improved.
| [html_version](/cells/python-net/aspose.cells/htmlsaveoptions/html_version) | Specifies version of HTML standard that should be used when saving the HTML format.
| [sheet_set](/cells/python-net/aspose.cells/htmlsaveoptions/sheet_set) | Gets or sets the sheets to render. Default is all visible sheets in the workbook: [`SheetSet.visible`](/cells/python-net/aspose.cells.rendering/sheetset#visible). |
### See Also
* module [`aspose.cells`](..)
* class [`HtmlSaveOptions`](/cells/python-net/aspose.cells/htmlsaveoptions)
* class [`SaveOptions`](/cells/python-net/aspose.cells/saveoptions)
