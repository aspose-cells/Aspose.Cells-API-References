---
title: XpsSaveOptions class
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 1720
url: /python-net/aspose.cells/xpssaveoptions/
is_root: false
---

## XpsSaveOptions class

Represents the additional options when saving the file as the Xps.



**Inheritance:** [XpsSaveOptions](/cells/python-net/aspose.cells/xpssaveoptions) → 
[PaginatedSaveOptions](/cells/python-net/aspose.cells/paginatedsaveoptions) → 
[SaveOptions](/cells/python-net/aspose.cells/saveoptions)



The XpsSaveOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [XpsSaveOptions()](/cells/python-net/aspose.cells/xpssaveoptions/__init__/#) | Creates options for saving xps file. |
| [XpsSaveOptions(save_format)](/cells/python-net/aspose.cells/xpssaveoptions/__init__/#SaveFormat) | Creates options for saving xps file. |


### Properties
| Property | Description |
| :- | :- |
| [save_format](/cells/python-net/aspose.cells/xpssaveoptions/save_format) | Gets the save file format. |
| [clear_data](/cells/python-net/aspose.cells/xpssaveoptions/clear_data) | Make the workbook empty after saving the file. |
| [cached_file_folder](/cells/python-net/aspose.cells/xpssaveoptions/cached_file_folder) | The cached file folder is used to store some large data. |
| [validate_merged_areas](/cells/python-net/aspose.cells/xpssaveoptions/validate_merged_areas) | Indicates whether validate merged cells before saving the file. |
| [merge_areas](/cells/python-net/aspose.cells/xpssaveoptions/merge_areas) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [create_directory](/cells/python-net/aspose.cells/xpssaveoptions/create_directory) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [sort_names](/cells/python-net/aspose.cells/xpssaveoptions/sort_names) | Indicates whether sorting defined names before saving file. |
| [sort_external_names](/cells/python-net/aspose.cells/xpssaveoptions/sort_external_names) | Indicates whether sorting external defined names before saving file. |
| [refresh_chart_cache](/cells/python-net/aspose.cells/xpssaveoptions/refresh_chart_cache) | Indicates whether refreshing chart cache data |
| [warning_callback](/cells/python-net/aspose.cells/xpssaveoptions/warning_callback) | Gets or sets warning callback. |
| [update_smart_art](/cells/python-net/aspose.cells/xpssaveoptions/update_smart_art) | Indicates whether updating smart art setting.<br/>The default value is false. |
| [default_font](/cells/python-net/aspose.cells/xpssaveoptions/default_font) | When characters in the Excel are Unicode and not be set with correct font in cell style,<br/>They may appear as block in pdf,image.<br/>Set the DefaultFont such as MingLiu or MS Gothic to show these characters.<br/>If this property is not set, Aspose.Cells will use system default font to show these unicode characters. |
| [check_workbook_default_font](/cells/python-net/aspose.cells/xpssaveoptions/check_workbook_default_font) | When characters in the Excel are Unicode and not be set with correct font in cell style,<br/>They may appear as block in pdf,image.<br/>Set this to true to try to use workbook's default font to show these characters first. |
| [check_font_compatibility](/cells/python-net/aspose.cells/xpssaveoptions/check_font_compatibility) | Indicates whether to check font compatibility for every character in text. |
| [is_font_substitution_char_granularity](/cells/python-net/aspose.cells/xpssaveoptions/is_font_substitution_char_granularity) | Indicates whether to only substitute the font of character when the cell font is not compatibility for it. |
| [one_page_per_sheet](/cells/python-net/aspose.cells/xpssaveoptions/one_page_per_sheet) | If OnePagePerSheet is true , all content of one sheet will output to only one page in result. <br/>The paper size of pagesetup will be invalid, and the other settings of pagesetup <br/>will still take effect. |
| [all_columns_in_one_page_per_sheet](/cells/python-net/aspose.cells/xpssaveoptions/all_columns_in_one_page_per_sheet) | If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. <br/>The width of paper size of pagesetup will be ignored, and the other settings of pagesetup <br/>will still take effect. |
| [ignore_error](/cells/python-net/aspose.cells/xpssaveoptions/ignore_error) | Indicates if you need to hide the error while rendering.<br/>The error can be error in shape, image, chart rendering, etc. |
| [output_blank_page_when_nothing_to_print](/cells/python-net/aspose.cells/xpssaveoptions/output_blank_page_when_nothing_to_print) | Indicates whether to output a blank page when there is nothing to print. |
| [page_index](/cells/python-net/aspose.cells/xpssaveoptions/page_index) | Gets or sets the 0-based index of the first page to save. |
| [page_count](/cells/python-net/aspose.cells/xpssaveoptions/page_count) | Gets or sets the number of pages to save. |
| [printing_page_type](/cells/python-net/aspose.cells/xpssaveoptions/printing_page_type) | Indicates which pages will not be printed. |
| [gridline_type](/cells/python-net/aspose.cells/xpssaveoptions/gridline_type) | Gets or sets gridline type. |
| [text_cross_type](/cells/python-net/aspose.cells/xpssaveoptions/text_cross_type) | Gets or sets displaying text type when the text width is larger than cell width. |
| [default_edit_language](/cells/python-net/aspose.cells/xpssaveoptions/default_edit_language) | Gets or sets default edit language. |
| [sheet_set](/cells/python-net/aspose.cells/xpssaveoptions/sheet_set) | Gets or sets the sheets to render. Default is all visible sheets in the workbook: [SheetSet.visible](/cells/python-net/aspose.cells.rendering/sheetset#visible). |
| [draw_object_event_handler](/cells/python-net/aspose.cells/xpssaveoptions/draw_object_event_handler) | Implements this interface to get DrawObject and Bound when rendering. |
| [page_saving_callback](/cells/python-net/aspose.cells/xpssaveoptions/page_saving_callback) | Control/Indicate progress of page saving process. |


### See Also

* module [aspose.cells](../)
* class [PaginatedSaveOptions](/cells/python-net/aspose.cells/paginatedsaveoptions)
