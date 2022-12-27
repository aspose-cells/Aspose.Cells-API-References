---
title: AbstractTextLoadOptions class
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 60
url: /python-net/aspose.cells/abstracttextloadoptions/
is_root: false
---

## AbstractTextLoadOptions class

Common options for loading text values



**Inheritance:** [AbstractTextLoadOptions](/cells/python-net/aspose.cells/abstracttextloadoptions) → 
[LoadOptions](/cells/python-net/aspose.cells/loadoptions)



The AbstractTextLoadOptions type exposes the following members:

### Properties
| Property | Description |
| :- | :- |
| [load_format](/cells/python-net/aspose.cells/abstracttextloadoptions/load_format) | Gets the load format. |
| [password](/cells/python-net/aspose.cells/abstracttextloadoptions/password) | Gets and set the password of the workbook. |
| [parsing_formula_on_open](/cells/python-net/aspose.cells/abstracttextloadoptions/parsing_formula_on_open) | Indicates whether parsing the formula when reading the file. |
| [parsing_pivot_cached_records](/cells/python-net/aspose.cells/abstracttextloadoptions/parsing_pivot_cached_records) | Indicates whether parsing pivot cached records when loading the file.<br/>The default value is false. |
| [language_code](/cells/python-net/aspose.cells/abstracttextloadoptions/language_code) | Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. |
| [region](/cells/python-net/aspose.cells/abstracttextloadoptions/region) | Gets or sets the system regional settings based on CountryCode at the time the file was loaded. |
| [default_style_settings](/cells/python-net/aspose.cells/abstracttextloadoptions/default_style_settings) | Gets the default style settings for initializing styles of the workbook |
| [standard_font](/cells/python-net/aspose.cells/abstracttextloadoptions/standard_font) | Sets the default standard font name |
| [standard_font_size](/cells/python-net/aspose.cells/abstracttextloadoptions/standard_font_size) | Sets the default standard font size. |
| [interrupt_monitor](/cells/python-net/aspose.cells/abstracttextloadoptions/interrupt_monitor) | Gets and sets the interrupt monitor. |
| [ignore_not_printed](/cells/python-net/aspose.cells/abstracttextloadoptions/ignore_not_printed) | Ignore the data which are not printed if directly printing the file |
| [check_data_valid](/cells/python-net/aspose.cells/abstracttextloadoptions/check_data_valid) | Check whether data is valid in the template file. |
| [check_excel_restriction](/cells/python-net/aspose.cells/abstracttextloadoptions/check_excel_restriction) | Whether check restriction of excel file when user modify cells related objects.<br/>For example, excel does not allow inputting string value longer than 32K.<br/>When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception.<br/>If this property is false, we will accept your input string value as the cell's value so that later<br/>you can output the complete string value for other file formats such as CSV.<br/>However, if you have set such kind of value that is invalid for excel file format,<br/>you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file. |
| [keep_unparsed_data](/cells/python-net/aspose.cells/abstracttextloadoptions/keep_unparsed_data) | Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true. |
| [load_filter](/cells/python-net/aspose.cells/abstracttextloadoptions/load_filter) | The filter to denote how to load data. |
| [light_cells_data_handler](/cells/python-net/aspose.cells/abstracttextloadoptions/light_cells_data_handler) | The data handler for processing cells data when reading template file. |
| [memory_setting](/cells/python-net/aspose.cells/abstracttextloadoptions/memory_setting) | Gets or sets the memory usage options. |
| [warning_callback](/cells/python-net/aspose.cells/abstracttextloadoptions/warning_callback) | Gets or sets warning callback. |
| [auto_fitter_options](/cells/python-net/aspose.cells/abstracttextloadoptions/auto_fitter_options) | Gets and sets the auto fitter options |
| [auto_filter](/cells/python-net/aspose.cells/abstracttextloadoptions/auto_filter) | Indicates whether auto filtering the data when loading the files. |
| [font_configs](/cells/python-net/aspose.cells/abstracttextloadoptions/font_configs) | Gets and sets individual font configs. <br/>Only works for the [Workbook](/cells/python-net/aspose.cells/workbook) which uses this [LoadOptions](/cells/python-net/aspose.cells/loadoptions) to load. |
| [encoding](/cells/python-net/aspose.cells/abstracttextloadoptions/encoding) | Gets and sets the default encoding. Only applies for csv file. |
| [load_style_strategy](/cells/python-net/aspose.cells/abstracttextloadoptions/load_style_strategy) | Indicates the strategy to apply style for parsed values when converting string value to number or datetime. |
| [convert_numeric_data](/cells/python-net/aspose.cells/abstracttextloadoptions/convert_numeric_data) | Gets or sets a value that indicates whether the string in text file is converted to numeric data. |
| [convert_date_time_data](/cells/python-net/aspose.cells/abstracttextloadoptions/convert_date_time_data) | Gets or sets a value that indicates whether the string in text file is converted to date data. |
| [keep_precision](/cells/python-net/aspose.cells/abstracttextloadoptions/keep_precision) | Indicates whether not parsing a string value if the length is 15. |


### Methods
| Method | Description |
| :- | :- |
| [set_paper_size(type)](/cells/python-net/aspose.cells/abstracttextloadoptions/set_paper_size/#PaperSizeType) | Sets the default print paper size from default printer's setting. |


### See Also

* module [aspose.cells](../)
* class [LoadOptions](/cells/python-net/aspose.cells/loadoptions)
