---
title: TxtSaveOptions class
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 1520
url: /python-net/aspose.cells/txtsaveoptions/
is_root: false
---

## TxtSaveOptions class

Represents the save options for csv/tab delimited/other text format.



**Inheritance:** [TxtSaveOptions](/cells/python-net/aspose.cells/txtsaveoptions) → 
[SaveOptions](/cells/python-net/aspose.cells/saveoptions)



The TxtSaveOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [TxtSaveOptions()](/cells/python-net/aspose.cells/txtsaveoptions/__init__/#) | Creates text file save options. |
| [TxtSaveOptions(format)](/cells/python-net/aspose.cells/txtsaveoptions/__init__/#SaveFormat) | Creates text file save options. |


### Properties
| Property | Description |
| :- | :- |
| [save_format](/cells/python-net/aspose.cells/txtsaveoptions/save_format) | Gets the save file format. |
| [clear_data](/cells/python-net/aspose.cells/txtsaveoptions/clear_data) | Make the workbook empty after saving the file. |
| [cached_file_folder](/cells/python-net/aspose.cells/txtsaveoptions/cached_file_folder) | The cached file folder is used to store some large data. |
| [validate_merged_areas](/cells/python-net/aspose.cells/txtsaveoptions/validate_merged_areas) | Indicates whether validate merged cells before saving the file. |
| [merge_areas](/cells/python-net/aspose.cells/txtsaveoptions/merge_areas) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [create_directory](/cells/python-net/aspose.cells/txtsaveoptions/create_directory) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [sort_names](/cells/python-net/aspose.cells/txtsaveoptions/sort_names) | Indicates whether sorting defined names before saving file. |
| [sort_external_names](/cells/python-net/aspose.cells/txtsaveoptions/sort_external_names) | Indicates whether sorting external defined names before saving file. |
| [refresh_chart_cache](/cells/python-net/aspose.cells/txtsaveoptions/refresh_chart_cache) | Indicates whether refreshing chart cache data |
| [warning_callback](/cells/python-net/aspose.cells/txtsaveoptions/warning_callback) | Gets or sets warning callback. |
| [update_smart_art](/cells/python-net/aspose.cells/txtsaveoptions/update_smart_art) | Indicates whether updating smart art setting.<br/>The default value is false. |
| [separator](/cells/python-net/aspose.cells/txtsaveoptions/separator) | Gets and sets char Delimiter of text file. |
| [separator_string](/cells/python-net/aspose.cells/txtsaveoptions/separator_string) | Gets and sets a string value as separator. |
| [encoding](/cells/python-net/aspose.cells/txtsaveoptions/encoding) | Gets and sets the default encoding. |
| [always_quoted](/cells/python-net/aspose.cells/txtsaveoptions/always_quoted) | Indicates whether always adding '"' for each field.<br/>If true then all values will be quoted;<br/>If false then values will only be quoted when needed(for example,<br/>when values contain special characters such as '"' , '\n' or separator character).<br/>Default is false. |
| [quote_type](/cells/python-net/aspose.cells/txtsaveoptions/quote_type) | Gets or sets how to quote values in the exported text file. |
| [format_strategy](/cells/python-net/aspose.cells/txtsaveoptions/format_strategy) | Gets and sets the format strategy when exporting the cell value as string. |
| [light_cells_data_provider](/cells/python-net/aspose.cells/txtsaveoptions/light_cells_data_provider) | The Data provider to provide cells data for saving workbook in light mode. |
| [trim_leading_blank_row_and_column](/cells/python-net/aspose.cells/txtsaveoptions/trim_leading_blank_row_and_column) | Indicates whether leading blank rows and columns should be trimmed like what ms excel does.<br/>Default is true. |
| [trim_tailing_blank_cells](/cells/python-net/aspose.cells/txtsaveoptions/trim_tailing_blank_cells) | Indicates whether tailing blank cells in one row should be trimmed. Default is false. |
| [keep_separators_for_blank_row](/cells/python-net/aspose.cells/txtsaveoptions/keep_separators_for_blank_row) | Indicates whether separators should be output for blank row.<br/>Default value is false so by default the content for blank row will be empty. |
| [export_area](/cells/python-net/aspose.cells/txtsaveoptions/export_area) | The range of cells to be exported. |
| [export_quote_prefix](/cells/python-net/aspose.cells/txtsaveoptions/export_quote_prefix) | Indicates whether the single quote sign should be exported as part of the value of one cell<br/>when [Style.quote_prefix](/cells/python-net/aspose.cells/style#quote_prefix) is true for it. Default is false. |
| [export_all_sheets](/cells/python-net/aspose.cells/txtsaveoptions/export_all_sheets) | Indicates whether exporting all sheets to the text file.<br/>If it is false, only export the activesheet, just like MS Excel. |



### See Also
* module [aspose.cells](..)
* class [SaveOptions](/cells/python-net/aspose.cells/saveoptions)
* class [TxtSaveOptions](/cells/python-net/aspose.cells/txtsaveoptions)
