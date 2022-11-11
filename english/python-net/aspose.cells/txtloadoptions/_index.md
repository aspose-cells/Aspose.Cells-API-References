---
title: TxtLoadOptions
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 1500
url: /python-net/aspose.cells/txtloadoptions/
---

## TxtLoadOptions class

Represents the options for loading text file.

The TxtLoadOptions type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|TxtLoadOptions()|Creates the options for loading text file.|
|TxtLoadOptions(load_format)|Initializes a new instance of the TxtLoadOptions class|
## Properties
| Name | Description |
| :- | :- |
|load_format|  |
|password|  |
|parsing_formula_on_open|  |
|parsing_pivot_cached_records|  |
|language_code|  |
|region|  |
|default_style_settings|  |
|standard_font|  |
|standard_font_size|  |
|interrupt_monitor|  |
|ignore_not_printed|  |
|check_data_valid|  |
|check_excel_restriction|  |
|keep_unparsed_data|  |
|load_filter|  |
|light_cells_data_handler|  |
|memory_setting|  |
|warning_callback|  |
|auto_fitter_options|  |
|auto_filter|  |
|font_configs|  |
|encoding|Gets and sets the default encoding. Only applies for csv file.|
|load_style_strategy|Indicates the strategy to apply style for parsed values when converting string value to number or datetime.|
|convert_numeric_data|Gets or sets a value that indicates whether the string in text file is converted to numeric data.|
|convert_date_time_data|Gets or sets a value that indicates whether the string in text file is converted to date data.|
|keep_precision|Indicates whether not parsing a string value if the length is 15.|
|separator|Gets and sets character separator of text file.|
|separator_string|Gets and sets a string value as separator.|
|is_multi_encoded|True means that the file contains several encoding.|
|preferred_parsers|Gets and sets preferred value parsers for loading text file.|
|has_formula|Indicates whether the text is formula if it starts with "=".|
|has_text_qualifier|Whether there is text qualifier for cell value. Default is true.|
|text_qualifier|Specifies the text qualifier for cell values. Default qualifier is '"'.|
|treat_consecutive_delimiters_as_one|Whether consecutive delimiters should be treated as one.|
|treat_quote_prefix_as_value|Indicates whether the leading single quote sign should be taken as part of the value of one cell.<br/>            Default is true. If it is false, the leading single quote will be removed from corresponding cell's value<br/>            and [quote_prefix](/python-net/aspose.cells/style/) will be set as true for the cell.|
|extend_to_next_sheet|Whether extends data to next sheet when the rows or columns of data exceed limit.<br/>            If this property is true, extra data will be extended to next sheet behind current one(if current sheet is the last one,<br/>            new sheet will be appended to current workbook).<br/>            If this property is false, the data exceeds limit will be ignored.<br/>            Default is false;|
## Methods
| Name | Description |
| :- | :- |
|set_paper_size(type)|  |

### See Also

* namespace [aspose.cells](/python-net/aspose.cells/)
* assembly [Aspose.Cells](/python-net/)

