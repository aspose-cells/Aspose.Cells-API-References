##CellsHelper class
## CellsHelper class
Provides helper functions.
The CellsHelper type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [significant_digits](/cells/python-net/aspose.cells/cellshelper/significant_digits) | Gets and sets the number of significant digits.
| [dpi](/cells/python-net/aspose.cells/cellshelper/dpi) | Gets the DPI of the machine. |
| [startup_path](/cells/python-net/aspose.cells/cellshelper/startup_path) | Gets or sets the startup path, which is referred to by some external formula references. |
| [alt_start_path](/cells/python-net/aspose.cells/cellshelper/alt_start_path) | Gets or sets the alternate startup path, which is referred to by some external formula references. |
| [library_path](/cells/python-net/aspose.cells/cellshelper/library_path) | Gets or sets the library path which is referred to by some external formula references. |
| [custom_implementation_factory](/cells/python-net/aspose.cells/cellshelper/custom_implementation_factory) | Gets or sets the factory for creating instances with special implementation. |
| [is_cloud_platform](/cells/python-net/aspose.cells/cellshelper/is_cloud_platform) | Please set this property True when running on a cloud platform, such as: Azure, AWSLambda, etc, |
### Methods
| Method | Description |
| :- | :- |
| [`create_safe_sheet_name(, name_proposal)`](/cells/python-net/aspose.cells/cellshelper/create_safe_sheet_name/#system.string) | Checks given sheet name and create a valid one when needed.
| [`create_safe_sheet_name(, name_proposal, replace_char)`](/cells/python-net/aspose.cells/cellshelper/create_safe_sheet_name/#system.string-system.char) | Checks given sheet name and create a valid one when needed.
| [`get_text_width(, text, font, scaling)`](/cells/python-net/aspose.cells/cellshelper/get_text_width/#system.string-aspose.cells.font-float) | Get width of text in unit of points. |
| [`get_version()`](/cells/python-net/aspose.cells/cellshelper/get_version/#) | Get the release version. |
| [`cell_name_to_index(, cell_name, row, column)`](/cells/python-net/aspose.cells/cellshelper/cell_name_to_index/#system.string-any-any) | Gets the cell row and column indexes according to its name. |
| [`cell_index_to_name(, row, column)`](/cells/python-net/aspose.cells/cellshelper/cell_index_to_name/#int-int) | Gets cell name according to its row and column indexes. |
| [`column_index_to_name(, column)`](/cells/python-net/aspose.cells/cellshelper/column_index_to_name/#int) | Gets column name according to column index. |
| [`column_name_to_index(, column_name)`](/cells/python-net/aspose.cells/cellshelper/column_name_to_index/#system.string) | Gets column index according to column name. |
| [`row_index_to_name(, row)`](/cells/python-net/aspose.cells/cellshelper/row_index_to_name/#int) | Gets row name according to row index. |
| [`row_name_to_index(, row_name)`](/cells/python-net/aspose.cells/cellshelper/row_name_to_index/#system.string) | Gets row index according to row name. |
| [`convert_r1c1_formula_to_a1(, r_1c1_formula, row, column)`](/cells/python-net/aspose.cells/cellshelper/convert_r1c1_formula_to_a1/#system.string-int-int) | Converts the r1c1 formula of the cell to A1 formula. |
| [`convert_a1_formula_to_r1c1(, formula, row, column)`](/cells/python-net/aspose.cells/cellshelper/convert_a1_formula_to_r1c1/#system.string-int-int) | Converts A1 formula of the cell to the r1c1 formula. |
| [`get_date_time_from_double(, double_value, date1904)`](/cells/python-net/aspose.cells/cellshelper/get_date_time_from_double/#float-bool) | Convert the double value to the date time value. |
| [`get_double_from_date_time(, date_time, date1904)`](/cells/python-net/aspose.cells/cellshelper/get_double_from_date_time/#system.datetime-bool) | Convert the date time to double value. |
| [`get_used_colors(, workbook)`](/cells/python-net/aspose.cells/cellshelper/get_used_colors/#aspose.cells.workbook) | Gets all used colors in the workbook. |
| [`add_add_in_function(, function, min_count_of_parameters, max_count_of_parameters, paramers_type, function_value_type)`](/cells/python-net/aspose.cells/cellshelper/add_add_in_function/#system.string-int-int-list-aspose.cells.parametertype) | Add addin function. |
| [`merge_files(, files, cached_file, dest_file)`](/cells/python-net/aspose.cells/cellshelper/merge_files/#list-system.string-system.string) | Merges some large xls files to a xls file. |
| [`get_cache_folder()`](/cells/python-net/aspose.cells/cellshelper/get_cache_folder/#) | Gets the folder for temporary files that may be used as data cache. |
| [`set_cache_folder(, cache)`](/cells/python-net/aspose.cells/cellshelper/set_cache_folder/#system.string) | Sets the folder for temporary files that may be used as data cache. |
| [`need_quote_in_formula(, sheet_name)`](/cells/python-net/aspose.cells/cellshelper/need_quote_in_formula/#system.string) | Indicates whether the name of the sheet should be enclosed in single quotes |
| [`init_for_dot_net_core()`](/cells/python-net/aspose.cells/cellshelper/init_for_dot_net_core/#) | Do the initialization for .NetCore programme.
### See Also
* module [`aspose.cells`](..)
