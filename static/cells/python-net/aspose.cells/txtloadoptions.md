##TxtLoadOptions class
## TxtLoadOptions class
Represents the options for loading text file.
**Inheritance:** [`TxtLoadOptions`](/cells/python-net/aspose.cells/txtloadoptions) →
[`AbstractTextLoadOptions`](/cells/python-net/aspose.cells/abstracttextloadoptions) →
[`LoadOptions`](/cells/python-net/aspose.cells/loadoptions)
The TxtLoadOptions type exposes the following members:
### Constructors
| Constructor | Description |
| :- | :- |
| [`__init__(self)`](/cells/python-net/aspose.cells/txtloadoptions/__init__/#) | Creates the options for loading text file. |
| [`__init__(self, load_format)`](/cells/python-net/aspose.cells/txtloadoptions/__init__/#aspose.cells.loadformat) | Creates the options for loading text file. |
### Properties
| Property | Description |
| :- | :- |
| [load_format](/cells/python-net/aspose.cells/txtloadoptions/load_format) | Gets the load format. |
| [password](/cells/python-net/aspose.cells/txtloadoptions/password) | Gets and set the password of the workbook. |
| [parsing_formula_on_open](/cells/python-net/aspose.cells/txtloadoptions/parsing_formula_on_open) | Indicates whether parsing the formula when reading the file. |
| [parsing_pivot_cached_records](/cells/python-net/aspose.cells/txtloadoptions/parsing_pivot_cached_records) | Indicates whether parsing pivot cached records when loading the file.
| [language_code](/cells/python-net/aspose.cells/txtloadoptions/language_code) | Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. |
| [region](/cells/python-net/aspose.cells/txtloadoptions/region) | Gets or sets the regional settings used for the Workbook that will be loaded. |
| [default_style_settings](/cells/python-net/aspose.cells/txtloadoptions/default_style_settings) | Gets the default style settings for initializing styles of the workbook |
| [standard_font](/cells/python-net/aspose.cells/txtloadoptions/standard_font) | Sets the default standard font name |
| [standard_font_size](/cells/python-net/aspose.cells/txtloadoptions/standard_font_size) | Sets the default standard font size. |
| [interrupt_monitor](/cells/python-net/aspose.cells/txtloadoptions/interrupt_monitor) | Gets and sets the interrupt monitor. |
| [ignore_not_printed](/cells/python-net/aspose.cells/txtloadoptions/ignore_not_printed) | Ignore the data which are not printed if directly printing the file |
| [check_data_valid](/cells/python-net/aspose.cells/txtloadoptions/check_data_valid) | Check whether data is valid in the template file. |
| [check_excel_restriction](/cells/python-net/aspose.cells/txtloadoptions/check_excel_restriction) | Whether check restriction of excel file when user modify cells related objects.
| [keep_unparsed_data](/cells/python-net/aspose.cells/txtloadoptions/keep_unparsed_data) | Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true. |
| [load_filter](/cells/python-net/aspose.cells/txtloadoptions/load_filter) | The filter to denote how to load data. |
| [light_cells_data_handler](/cells/python-net/aspose.cells/txtloadoptions/light_cells_data_handler) | The data handler for processing cells data when reading template file. |
| [memory_setting](/cells/python-net/aspose.cells/txtloadoptions/memory_setting) | Gets or sets the memory mode for loaded workbook. |
| [warning_callback](/cells/python-net/aspose.cells/txtloadoptions/warning_callback) | Gets or sets warning callback. |
| [auto_fitter_options](/cells/python-net/aspose.cells/txtloadoptions/auto_fitter_options) | Gets and sets the auto fitter options |
| [auto_filter](/cells/python-net/aspose.cells/txtloadoptions/auto_filter) | Indicates whether auto filtering the data when loading the files. |
| [font_configs](/cells/python-net/aspose.cells/txtloadoptions/font_configs) | Gets and sets individual font configs.
| [ignore_useless_shapes](/cells/python-net/aspose.cells/txtloadoptions/ignore_useless_shapes) | Indicates whether ignoring useless shapes. |
| [preserve_padding_spaces_in_formula](/cells/python-net/aspose.cells/txtloadoptions/preserve_padding_spaces_in_formula) | Indicates whether preserve those spaces and line breaks that are padded between formula tokens
| [encoding](/cells/python-net/aspose.cells/txtloadoptions/encoding) | Gets and sets the default encoding. Only applies for csv file. |
| [load_style_strategy](/cells/python-net/aspose.cells/txtloadoptions/load_style_strategy) | Indicates the strategy to apply style for parsed values when converting string value to number or datetime. |
| [convert_numeric_data](/cells/python-net/aspose.cells/txtloadoptions/convert_numeric_data) | Gets or sets a value that indicates whether the string in text file is converted to numeric data. |
| [convert_date_time_data](/cells/python-net/aspose.cells/txtloadoptions/convert_date_time_data) | Gets or sets a value that indicates whether the string in text file is converted to date data. |
| [keep_precision](/cells/python-net/aspose.cells/txtloadoptions/keep_precision) | Indicates whether not parsing a string value if the length is 15. |
| [separator](/cells/python-net/aspose.cells/txtloadoptions/separator) | Gets and sets character separator of text file. |
| [separator_string](/cells/python-net/aspose.cells/txtloadoptions/separator_string) | Gets and sets a string value as separator. |
| [is_multi_encoded](/cells/python-net/aspose.cells/txtloadoptions/is_multi_encoded) | True means that the file contains several encoding. |
| [preferred_parsers](/cells/python-net/aspose.cells/txtloadoptions/preferred_parsers) | Gets and sets preferred value parsers for loading text file. |
| [has_formula](/cells/python-net/aspose.cells/txtloadoptions/has_formula) | Indicates whether the text is formula if it starts with "=". |
| [has_text_qualifier](/cells/python-net/aspose.cells/txtloadoptions/has_text_qualifier) | Whether there is text qualifier for cell value. Default is true. |
| [text_qualifier](/cells/python-net/aspose.cells/txtloadoptions/text_qualifier) | Specifies the text qualifier for cell values. Default qualifier is '"'. |
| [treat_consecutive_delimiters_as_one](/cells/python-net/aspose.cells/txtloadoptions/treat_consecutive_delimiters_as_one) | Whether consecutive delimiters should be treated as one. |
| [treat_quote_prefix_as_value](/cells/python-net/aspose.cells/txtloadoptions/treat_quote_prefix_as_value) | Indicates whether the leading single quote sign should be taken as part of the value of one cell.
| [extend_to_next_sheet](/cells/python-net/aspose.cells/txtloadoptions/extend_to_next_sheet) | Whether extends data to next sheet when the rows or columns of data exceed limit.
| [header_rows_count](/cells/python-net/aspose.cells/txtloadoptions/header_rows_count) | The count of header rows to be repeated for extended sheets. |
| [header_columns_count](/cells/python-net/aspose.cells/txtloadoptions/header_columns_count) | The count of header columns to be repeated for extended sheets. |
| [max_row_count](/cells/python-net/aspose.cells/txtloadoptions/max_row_count) | The maximum count of rows to be imported for one sheet. |
| [max_column_count](/cells/python-net/aspose.cells/txtloadoptions/max_column_count) | The maximum count of columns to be imported for one sheet. |
### Methods
| Method | Description |
| :- | :- |
| [`set_paper_size(self, type)`](/cells/python-net/aspose.cells/txtloadoptions/set_paper_size/#aspose.cells.papersizetype) | Sets the default print paper size from default printer's setting. |
### See Also
* module [`aspose.cells`](..)
* class [`AbstractTextLoadOptions`](/cells/python-net/aspose.cells/abstracttextloadoptions)
* class [`LoadOptions`](/cells/python-net/aspose.cells/loadoptions)
* class [`TxtLoadOptions`](/cells/python-net/aspose.cells/txtloadoptions)
* class [`Workbook`](/cells/python-net/aspose.cells/workbook)
