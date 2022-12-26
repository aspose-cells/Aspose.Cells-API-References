---
title: JsonLoadOptions class
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 960
url: /python-net/aspose.cells/jsonloadoptions/
is_root: false
---

## JsonLoadOptions class

Represents the options of loading json files



**Inheritance:** [JsonLoadOptions](/cells/python-net/aspose.cells/jsonloadoptions) → 
[LoadOptions](/cells/python-net/aspose.cells/loadoptions)



The JsonLoadOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [JsonLoadOptions()](/cells/python-net/aspose.cells/jsonloadoptions/__init__/#) | Creates an options of loading the file. |


### Properties
| Property | Description |
| :- | :- |
| [load_format](/cells/python-net/aspose.cells/jsonloadoptions/load_format) | Gets the load format. |
| [password](/cells/python-net/aspose.cells/jsonloadoptions/password) | Gets and set the password of the workbook. |
| [parsing_formula_on_open](/cells/python-net/aspose.cells/jsonloadoptions/parsing_formula_on_open) | Indicates whether parsing the formula when reading the file. |
| [parsing_pivot_cached_records](/cells/python-net/aspose.cells/jsonloadoptions/parsing_pivot_cached_records) | Indicates whether parsing pivot cached records when loading the file.<br/>The default value is false. |
| [language_code](/cells/python-net/aspose.cells/jsonloadoptions/language_code) | Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. |
| [region](/cells/python-net/aspose.cells/jsonloadoptions/region) | Gets or sets the system regional settings based on CountryCode at the time the file was loaded. |
| [default_style_settings](/cells/python-net/aspose.cells/jsonloadoptions/default_style_settings) | Gets the default style settings for initializing styles of the workbook |
| [standard_font](/cells/python-net/aspose.cells/jsonloadoptions/standard_font) | Sets the default standard font name |
| [standard_font_size](/cells/python-net/aspose.cells/jsonloadoptions/standard_font_size) | Sets the default standard font size. |
| [interrupt_monitor](/cells/python-net/aspose.cells/jsonloadoptions/interrupt_monitor) | Gets and sets the interrupt monitor. |
| [ignore_not_printed](/cells/python-net/aspose.cells/jsonloadoptions/ignore_not_printed) | Ignore the data which are not printed if directly printing the file |
| [check_data_valid](/cells/python-net/aspose.cells/jsonloadoptions/check_data_valid) | Check whether data is valid in the template file. |
| [check_excel_restriction](/cells/python-net/aspose.cells/jsonloadoptions/check_excel_restriction) | Whether check restriction of excel file when user modify cells related objects.<br/>For example, excel does not allow inputting string value longer than 32K.<br/>When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception.<br/>If this property is false, we will accept your input string value as the cell's value so that later<br/>you can output the complete string value for other file formats such as CSV.<br/>However, if you have set such kind of value that is invalid for excel file format,<br/>you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file. |
| [keep_unparsed_data](/cells/python-net/aspose.cells/jsonloadoptions/keep_unparsed_data) | Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true. |
| [load_filter](/cells/python-net/aspose.cells/jsonloadoptions/load_filter) | The filter to denote how to load data. |
| [light_cells_data_handler](/cells/python-net/aspose.cells/jsonloadoptions/light_cells_data_handler) | The data handler for processing cells data when reading template file. |
| [memory_setting](/cells/python-net/aspose.cells/jsonloadoptions/memory_setting) | Gets or sets the memory usage options. |
| [warning_callback](/cells/python-net/aspose.cells/jsonloadoptions/warning_callback) | Gets or sets warning callback. |
| [auto_fitter_options](/cells/python-net/aspose.cells/jsonloadoptions/auto_fitter_options) | Gets and sets the auto fitter options |
| [auto_filter](/cells/python-net/aspose.cells/jsonloadoptions/auto_filter) | Indicates whether auto filtering the data when loading the files. |
| [font_configs](/cells/python-net/aspose.cells/jsonloadoptions/font_configs) | Gets and sets individual font configs. <br/>Only works for the [Workbook](/cells/python-net/aspose.cells/workbook) which uses this [LoadOptions](/cells/python-net/aspose.cells/loadoptions) to load. |
| [start_cell](/cells/python-net/aspose.cells/jsonloadoptions/start_cell) | Gets and sets the start cell. |
| [layout_options](/cells/python-net/aspose.cells/jsonloadoptions/layout_options) | The options of import json. |
| [multiple_worksheets](/cells/python-net/aspose.cells/jsonloadoptions/multiple_worksheets) | Indicates whether importing each attribute of JsonObject object as one worksheet when all child nodes are array nodes. |


### Methods
| Method | Description |
| :- | :- |
| [set_paper_size(type)](/cells/python-net/aspose.cells/jsonloadoptions/set_paper_size/#PaperSizeType) | Sets the default print paper size from default printer's setting. |


### See Also

* module [aspose.cells](../)
* class [LoadOptions](/cells/python-net/aspose.cells/loadoptions)
