---
title: HtmlLoadOptions
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 770
url: /python-net/aspose.cells/htmlloadoptions/
---

## HtmlLoadOptions class

Represents options when importing a html file.

The HtmlLoadOptions type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|HtmlLoadOptions()|Creates an options of loading the file.|
|HtmlLoadOptions(load_format)|Initializes a new instance of the HtmlLoadOptions class|
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
|attached_files_directory|The directory that the attached files will be saved to.|
|load_formulas|Indicates whether importing formulas if the original html file contains formulas|
|support_div_tag|Indicates whether support the layout of <div> tag when the html file contains <div> tags. The default value is false.|
|delete_redundant_spaces|Indicates whether delete redundant spaces when the text wraps lines using <br>tag.The default value is false.|
|auto_fit_cols_and_rows|Indicates whether auto-fit columns and rows. The default value is false.|
|convert_formulas_data|if true, convert string to formula when string value starts with character '=',the default value is false.|
|stream_provider|Gets or sets the StreamProviderImportHtmlFile for importing objects.|
|prog_id|Gets the program id of creating the file.<br/>            Only for MHT files.|
## Methods
| Name | Description |
| :- | :- |
|set_paper_size(type)|  |

### See Also

* namespace [aspose.cells](/python-net/aspose.cells/)
* assembly [Aspose.Cells](/python-net/)

