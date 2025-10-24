##HtmlLoadOptions class
## HtmlLoadOptions class
Represents options when importing a html file.
**Inheritance:** [`HtmlLoadOptions`](/cells/python-net/aspose.cells/htmlloadoptions) →
[`AbstractTextLoadOptions`](/cells/python-net/aspose.cells/abstracttextloadoptions) →
[`LoadOptions`](/cells/python-net/aspose.cells/loadoptions)
The HtmlLoadOptions type exposes the following members:
### Constructors
| Constructor | Description |
| :- | :- |
| [`__init__(self)`](/cells/python-net/aspose.cells/htmlloadoptions/__init__/#) | Creates an options of loading the file. |
| [`__init__(self, load_format)`](/cells/python-net/aspose.cells/htmlloadoptions/__init__/#aspose.cells.loadformat) | Creates an options of loading the file. |
### Properties
| Property | Description |
| :- | :- |
| [load_format](/cells/python-net/aspose.cells/htmlloadoptions/load_format) | Gets the load format. |
| [password](/cells/python-net/aspose.cells/htmlloadoptions/password) | Gets and set the password of the workbook. |
| [parsing_formula_on_open](/cells/python-net/aspose.cells/htmlloadoptions/parsing_formula_on_open) | Indicates whether parsing the formula when reading the file. |
| [parsing_pivot_cached_records](/cells/python-net/aspose.cells/htmlloadoptions/parsing_pivot_cached_records) | Indicates whether parsing pivot cached records when loading the file.
| [language_code](/cells/python-net/aspose.cells/htmlloadoptions/language_code) | Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file. |
| [region](/cells/python-net/aspose.cells/htmlloadoptions/region) | Gets or sets the regional settings used for the Workbook that will be loaded. |
| [default_style_settings](/cells/python-net/aspose.cells/htmlloadoptions/default_style_settings) | Gets the default style settings for initializing styles of the workbook |
| [standard_font](/cells/python-net/aspose.cells/htmlloadoptions/standard_font) | Sets the default standard font name |
| [standard_font_size](/cells/python-net/aspose.cells/htmlloadoptions/standard_font_size) | Sets the default standard font size. |
| [interrupt_monitor](/cells/python-net/aspose.cells/htmlloadoptions/interrupt_monitor) | Gets and sets the interrupt monitor. |
| [ignore_not_printed](/cells/python-net/aspose.cells/htmlloadoptions/ignore_not_printed) | Ignore the data which are not printed if directly printing the file |
| [check_data_valid](/cells/python-net/aspose.cells/htmlloadoptions/check_data_valid) | Check whether data is valid in the template file. |
| [check_excel_restriction](/cells/python-net/aspose.cells/htmlloadoptions/check_excel_restriction) | Whether check restriction of excel file when user modify cells related objects.
| [keep_unparsed_data](/cells/python-net/aspose.cells/htmlloadoptions/keep_unparsed_data) | Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true. |
| [load_filter](/cells/python-net/aspose.cells/htmlloadoptions/load_filter) | The filter to denote how to load data. |
| [light_cells_data_handler](/cells/python-net/aspose.cells/htmlloadoptions/light_cells_data_handler) | The data handler for processing cells data when reading template file. |
| [memory_setting](/cells/python-net/aspose.cells/htmlloadoptions/memory_setting) | Gets or sets the memory mode for loaded workbook. |
| [warning_callback](/cells/python-net/aspose.cells/htmlloadoptions/warning_callback) | Gets or sets warning callback. |
| [auto_fitter_options](/cells/python-net/aspose.cells/htmlloadoptions/auto_fitter_options) | Gets and sets the auto fitter options |
| [auto_filter](/cells/python-net/aspose.cells/htmlloadoptions/auto_filter) | Indicates whether auto filtering the data when loading the files. |
| [font_configs](/cells/python-net/aspose.cells/htmlloadoptions/font_configs) | Gets and sets individual font configs.
| [ignore_useless_shapes](/cells/python-net/aspose.cells/htmlloadoptions/ignore_useless_shapes) | Indicates whether ignoring useless shapes. |
| [preserve_padding_spaces_in_formula](/cells/python-net/aspose.cells/htmlloadoptions/preserve_padding_spaces_in_formula) | Indicates whether preserve those spaces and line breaks that are padded between formula tokens
| [encoding](/cells/python-net/aspose.cells/htmlloadoptions/encoding) | Gets and sets the default encoding. Only applies for csv file. |
| [load_style_strategy](/cells/python-net/aspose.cells/htmlloadoptions/load_style_strategy) | Indicates the strategy to apply style for parsed values when converting string value to number or datetime. |
| [convert_numeric_data](/cells/python-net/aspose.cells/htmlloadoptions/convert_numeric_data) | Gets or sets a value that indicates whether the string in text file is converted to numeric data. |
| [convert_date_time_data](/cells/python-net/aspose.cells/htmlloadoptions/convert_date_time_data) | Gets or sets a value that indicates whether the string in text file is converted to date data. |
| [keep_precision](/cells/python-net/aspose.cells/htmlloadoptions/keep_precision) | Indicates whether not parsing a string value if the length is 15. |
| [attached_files_directory](/cells/python-net/aspose.cells/htmlloadoptions/attached_files_directory) | The directory that the attached files will be saved to. |
| [load_formulas](/cells/python-net/aspose.cells/htmlloadoptions/load_formulas) | Indicates whether importing formulas if the original html file contains formulas |
| [support_div_tag](/cells/python-net/aspose.cells/htmlloadoptions/support_div_tag) | Indicates whether support the layout of `<div>` tag when the html file contains it.
| [delete_redundant_spaces](/cells/python-net/aspose.cells/htmlloadoptions/delete_redundant_spaces) | Indicates whether delete redundant spaces when the text wraps lines using `<br>` tag.
| [auto_fit_cols_and_rows](/cells/python-net/aspose.cells/htmlloadoptions/auto_fit_cols_and_rows) | Indicates whether auto-fit columns and rows. The default value is false. |
| [convert_formulas_data](/cells/python-net/aspose.cells/htmlloadoptions/convert_formulas_data) | if true, convert string to formula when string value starts with character '=',the default value is false. |
| [has_formula](/cells/python-net/aspose.cells/htmlloadoptions/has_formula) | Indicates whether the text is formula if it starts with "=". |
| [stream_provider](/cells/python-net/aspose.cells/htmlloadoptions/stream_provider) | Gets or sets the StreamProviderImportHtmlFile for importing objects. |
| [prog_id](/cells/python-net/aspose.cells/htmlloadoptions/prog_id) | Gets the program id of creating the file.
| [table_load_options](/cells/python-net/aspose.cells/htmlloadoptions/table_load_options) | Get the HtmlTableLoadOptionCollection instance |
### Methods
| Method | Description |
| :- | :- |
| [`set_paper_size(self, type)`](/cells/python-net/aspose.cells/htmlloadoptions/set_paper_size/#aspose.cells.papersizetype) | Sets the default print paper size from default printer's setting. |
### See Also
* module [`aspose.cells`](..)
* class [`AbstractTextLoadOptions`](/cells/python-net/aspose.cells/abstracttextloadoptions)
* class [`HtmlLoadOptions`](/cells/python-net/aspose.cells/htmlloadoptions)
* class [`LoadOptions`](/cells/python-net/aspose.cells/loadoptions)
* class [`Workbook`](/cells/python-net/aspose.cells/workbook)
