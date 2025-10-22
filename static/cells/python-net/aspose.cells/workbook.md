##Workbook class
## Workbook class
Represents a root object to create an Excel spreadsheet.
The Workbook type exposes the following members:
### Constructors
| Constructor | Description |
| :- | :- |
| [`__init__(self)`](/cells/python-net/aspose.cells/workbook/__init__/#) | Initializes a new instance of the [`Workbook`](/cells/python-net/aspose.cells/workbook) class. |
| [`__init__(self, file_format_type)`](/cells/python-net/aspose.cells/workbook/__init__/#aspose.cells.fileformattype) | Initializes a new instance of the [`Workbook`](/cells/python-net/aspose.cells/workbook) class. |
| [`__init__(self, file)`](/cells/python-net/aspose.cells/workbook/__init__/#system.string) | Initializes a new instance of the [`Workbook`](/cells/python-net/aspose.cells/workbook) class and open a file. |
| [`__init__(self, stream)`](/cells/python-net/aspose.cells/workbook/__init__/#io.rawiobase) | Initializes a new instance of the [`Workbook`](/cells/python-net/aspose.cells/workbook) class and open a stream. |
| [`__init__(self, file, load_options)`](/cells/python-net/aspose.cells/workbook/__init__/#system.string-aspose.cells.loadoptions) | Initializes a new instance of the [`Workbook`](/cells/python-net/aspose.cells/workbook) class and open a file. |
| [`__init__(self, stream, load_options)`](/cells/python-net/aspose.cells/workbook/__init__/#io.rawiobase-aspose.cells.loadoptions) | Initializes a new instance of the [`Workbook`](/cells/python-net/aspose.cells/workbook) class and open stream. |
### Properties
| Property | Description |
| :- | :- |
| [settings](/cells/python-net/aspose.cells/workbook/settings) | Represents the workbook settings. |
| [worksheets](/cells/python-net/aspose.cells/workbook/worksheets) | Gets the [`WorksheetCollection`](/cells/python-net/aspose.cells/worksheetcollection) collection in the spreadsheet. |
| [is_licensed](/cells/python-net/aspose.cells/workbook/is_licensed) | Indicates whether license is set. |
| [colors](/cells/python-net/aspose.cells/workbook/colors) | Returns colors in the palette for the spreadsheet. |
| [count_of_styles_in_pool](/cells/python-net/aspose.cells/workbook/count_of_styles_in_pool) | Gets number of the styles in the style pool. |
| [default_style](/cells/python-net/aspose.cells/workbook/default_style) | Gets or sets the default [`Style`](/cells/python-net/aspose.cells/style) object of the workbook. |
| [is_digitally_signed](/cells/python-net/aspose.cells/workbook/is_digitally_signed) | Indicates if this spreadsheet is digitally signed. |
| [is_workbook_protected_with_password](/cells/python-net/aspose.cells/workbook/is_workbook_protected_with_password) | Indicates whether structure or window is protected with password. |
| [vba_project](/cells/python-net/aspose.cells/workbook/vba_project) | Gets the [`Workbook.vba_project`](/cells/python-net/aspose.cells/workbook#vba_project) in a spreadsheet. |
| [has_macro](/cells/python-net/aspose.cells/workbook/has_macro) | Indicates if this spreadsheet contains macro/VBA. |
| [has_revisions](/cells/python-net/aspose.cells/workbook/has_revisions) | Gets if the workbook has any tracked changes |
| [file_name](/cells/python-net/aspose.cells/workbook/file_name) | Gets and sets the current file name. |
| [cells_data_table_factory](/cells/python-net/aspose.cells/workbook/cells_data_table_factory) | Gets the factory for building ICellsDataTable from custom objects |
| [data_sorter](/cells/python-net/aspose.cells/workbook/data_sorter) | Gets a DataSorter object to sort data. |
| [theme](/cells/python-net/aspose.cells/workbook/theme) | Gets the theme name. |
| [built_in_document_properties](/cells/python-net/aspose.cells/workbook/built_in_document_properties) | Returns a [`DocumentProperty`](/cells/python-net/aspose.cells.properties/documentproperty) collection that represents all the built-in document properties of the spreadsheet. |
| [custom_document_properties](/cells/python-net/aspose.cells/workbook/custom_document_properties) | Returns a [`DocumentProperty`](/cells/python-net/aspose.cells.properties/documentproperty) collection that represents all the custom document properties of the spreadsheet. |
| [file_format](/cells/python-net/aspose.cells/workbook/file_format) | Gets and sets the file format. |
| [has_custom_function](/cells/python-net/aspose.cells/workbook/has_custom_function) | Detects whether there is custom function used in this workbook,
| [interrupt_monitor](/cells/python-net/aspose.cells/workbook/interrupt_monitor) | Gets and sets the interrupt monitor. |
| [content_type_properties](/cells/python-net/aspose.cells/workbook/content_type_properties) | Gets the list of  [`ContentTypeProperty`](/cells/python-net/aspose.cells.properties/contenttypeproperty) objects in the workbook. |
| [custom_xml_parts](/cells/python-net/aspose.cells/workbook/custom_xml_parts) | Represents a Custom XML Data Storage Part (custom XML data within a package). |
| [data_mashup](/cells/python-net/aspose.cells/workbook/data_mashup) | Gets mashup data. |
| [ribbon_xml](/cells/python-net/aspose.cells/workbook/ribbon_xml) | Gets and sets the XML file that defines the Ribbon UI. |
| [absolute_path](/cells/python-net/aspose.cells/workbook/absolute_path) | Gets and sets the absolute path of the file. |
| [data_connections](/cells/python-net/aspose.cells/workbook/data_connections) | Gets the ExternalConnection collection. |
| [data_model](/cells/python-net/aspose.cells/workbook/data_model) | Gets data model in the workbook. |
### Methods
| Method | Description |
| :- | :- |
| [`save(self, file_name, save_format)`](/cells/python-net/aspose.cells/workbook/save/#system.string-aspose.cells.saveformat) | Saves the workbook to the disk. |
| [`save(self, file_name)`](/cells/python-net/aspose.cells/workbook/save/#system.string) | Save the workbook to the disk. |
| [`save(self, file_name, save_options)`](/cells/python-net/aspose.cells/workbook/save/#system.string-aspose.cells.saveoptions) | Saves the workbook to the disk. |
| [`save(self, stream, save_format)`](/cells/python-net/aspose.cells/workbook/save/#io.rawiobase-aspose.cells.saveformat) | Saves the workbook to the stream. |
| [`save(self, stream, save_options)`](/cells/python-net/aspose.cells/workbook/save/#io.rawiobase-aspose.cells.saveoptions) | Saves the workbook to the stream. |
| [`create_style(self)`](/cells/python-net/aspose.cells/workbook/create_style/#) | Creates a new style. |
| [`create_style(self, clone_default_style)`](/cells/python-net/aspose.cells/workbook/create_style/#bool) | Creates a new style. |
| [`replace(self, place_holder, new_value)`](/cells/python-net/aspose.cells/workbook/replace/#system.string-system.string) | Replaces a cell's value with a new string. |
| [`replace(self, place_holder, new_value)`](/cells/python-net/aspose.cells/workbook/replace/#system.string-int) | Replaces a cell's value with a new integer. |
| [`replace(self, place_holder, new_value)`](/cells/python-net/aspose.cells/workbook/replace/#system.string-float) | Replaces a cell's value with a new double. |
| [`replace(self, place_holder, new_values, is_vertical)`](/cells/python-net/aspose.cells/workbook/replace/#system.string-list-bool) | Replaces a cell's value with a new string array. |
| [`replace(self, place_holder, new_values, is_vertical)`](/cells/python-net/aspose.cells/workbook/replace/#system.string-list-bool) | Replaces cells' values with an integer array. |
| [`replace(self, place_holder, new_values, is_vertical)`](/cells/python-net/aspose.cells/workbook/replace/#system.string-list-bool) | Replaces cells' values with a double array. |
| [`replace(self, bool_value, new_value)`](/cells/python-net/aspose.cells/workbook/replace/#bool-system.object) | Replaces cells' values with new data. |
| [`replace(self, int_value, new_value)`](/cells/python-net/aspose.cells/workbook/replace/#int-system.object) | Replaces cells' values with new data. |
| [`replace(self, place_holder, new_value, options)`](/cells/python-net/aspose.cells/workbook/replace/#system.string-system.string-aspose.cells.replaceoptions) | Replaces a cell's value with a new string. |
| [`copy(self, source, copy_options)`](/cells/python-net/aspose.cells/workbook/copy/#aspose.cells.workbook-aspose.cells.copyoptions) | Copies another Workbook object. |
| [`copy(self, source)`](/cells/python-net/aspose.cells/workbook/copy/#aspose.cells.workbook) | Copies data from a source Workbook object. |
| [`calculate_formula(self)`](/cells/python-net/aspose.cells/workbook/calculate_formula/#) | Calculates the result of formulas. |
| [`calculate_formula(self, ignore_error)`](/cells/python-net/aspose.cells/workbook/calculate_formula/#bool) | Calculates the result of formulas. |
| [`calculate_formula(self, options)`](/cells/python-net/aspose.cells/workbook/calculate_formula/#aspose.cells.calculationoptions) | Calculating formulas in this workbook. |
| [`refresh_dynamic_array_formulas(self, calculate)`](/cells/python-net/aspose.cells/workbook/refresh_dynamic_array_formulas/#bool) | Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data)
| [`refresh_dynamic_array_formulas(self, calculate, copts)`](/cells/python-net/aspose.cells/workbook/refresh_dynamic_array_formulas/#bool-aspose.cells.calculationoptions) | Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data) |
| [`import_xml(self, url, sheet_name, row, col)`](/cells/python-net/aspose.cells/workbook/import_xml/#system.string-system.string-int-int) | Imports/Updates an XML data file into the workbook. |
| [`import_xml(self, stream, sheet_name, row, col)`](/cells/python-net/aspose.cells/workbook/import_xml/#io.rawiobase-system.string-int-int) | Imports/Updates an XML data file into the workbook. |
| [`export_xml(self, map_name, path)`](/cells/python-net/aspose.cells/workbook/export_xml/#system.string-system.string) | Export XML data linked by the specified XML map. |
| [`export_xml(self, map_name, stream)`](/cells/python-net/aspose.cells/workbook/export_xml/#system.string-io.rawiobase) | Export XML data. |
| [`parse_formulas(self, ignore_error)`](/cells/python-net/aspose.cells/workbook/parse_formulas/#bool) | Parses all formulas which have not been parsed when they were loaded from template file or set to a cell. |
| [`start_access_cache(self, opts)`](/cells/python-net/aspose.cells/workbook/start_access_cache/#aspose.cells.accesscacheoptions) | Starts the session that uses caches to access data. |
| [`close_access_cache(self, opts)`](/cells/python-net/aspose.cells/workbook/close_access_cache/#aspose.cells.accesscacheoptions) | Closes the session that uses caches to access data. |
| [`remove_unused_styles(self)`](/cells/python-net/aspose.cells/workbook/remove_unused_styles/#) | Remove all unused styles. |
| [`create_builtin_style(self, type)`](/cells/python-net/aspose.cells/workbook/create_builtin_style/#aspose.cells.builtinstyletype) | Creates built-in style by given type. |
| [`create_cells_color(self)`](/cells/python-net/aspose.cells/workbook/create_cells_color/#) | Creates a [`CellsColor`](/cells/python-net/aspose.cells/cellscolor) object. |
| [`combine(self, second_workbook)`](/cells/python-net/aspose.cells/workbook/combine/#aspose.cells.workbook) | Combines another Workbook object. |
| [`get_style_in_pool(self, index)`](/cells/python-net/aspose.cells/workbook/get_style_in_pool/#int) | Gets the style in the style pool.
| [`get_fonts(self)`](/cells/python-net/aspose.cells/workbook/get_fonts/#) | Gets all fonts in the style pool. |
| [`get_named_style(self, name)`](/cells/python-net/aspose.cells/workbook/get_named_style/#system.string) | Gets the named style in the style pool. |
| [`merge_named_styles(self, source)`](/cells/python-net/aspose.cells/workbook/merge_named_styles/#aspose.cells.workbook) | Merges named styles from the other Excel file. |
| [`change_palette(self, color, index)`](/cells/python-net/aspose.cells/workbook/change_palette/#aspose.pydrawing.color-int) | Changes the palette for the spreadsheet in the specified index. |
| [`is_color_in_palette(self, color)`](/cells/python-net/aspose.cells/workbook/is_color_in_palette/#aspose.pydrawing.color) | Checks if a color is in the palette for the spreadsheet. |
| [`get_matching_color(self, raw_color)`](/cells/python-net/aspose.cells/workbook/get_matching_color/#aspose.pydrawing.color) | Find best matching Color in current palette. |
| [`set_encryption_options(self, encryption_type, key_length)`](/cells/python-net/aspose.cells/workbook/set_encryption_options/#aspose.cells.encryptiontype-int) | Set Encryption Options. |
| [`protect(self, protection_type, password)`](/cells/python-net/aspose.cells/workbook/protect/#aspose.cells.protectiontype-system.string) | Protects a workbook. |
| [`protect_shared_workbook(self, password)`](/cells/python-net/aspose.cells/workbook/protect_shared_workbook/#system.string) | Protects a shared workbook. |
| [`unprotect(self, password)`](/cells/python-net/aspose.cells/workbook/unprotect/#system.string) | Unprotects a workbook. |
| [`unprotect_shared_workbook(self, password)`](/cells/python-net/aspose.cells/workbook/unprotect_shared_workbook/#system.string) | Unprotects a shared workbook. |
| [`remove_macro(self)`](/cells/python-net/aspose.cells/workbook/remove_macro/#) | Removes VBA/macro from this spreadsheet. |
| [`remove_digital_signature(self)`](/cells/python-net/aspose.cells/workbook/remove_digital_signature/#) | Removes digital signature from this spreadsheet. |
| [`accept_all_revisions(self)`](/cells/python-net/aspose.cells/workbook/accept_all_revisions/#) | Accepts all tracked changes in the workbook. |
| [`remove_external_links(self)`](/cells/python-net/aspose.cells/workbook/remove_external_links/#) | Removes all external links in the workbook. |
| [`get_theme_color(self, type)`](/cells/python-net/aspose.cells/workbook/get_theme_color/#aspose.cells.themecolortype) | Gets theme color. |
| [`set_theme_color(self, type, color)`](/cells/python-net/aspose.cells/workbook/set_theme_color/#aspose.cells.themecolortype-aspose.pydrawing.color) | Sets the theme color |
| [`custom_theme(self, theme_name, colors)`](/cells/python-net/aspose.cells/workbook/custom_theme/#system.string-aspose.pydrawing.color[]) | Customs the theme. |
| [`copy_theme(self, source)`](/cells/python-net/aspose.cells/workbook/copy_theme/#aspose.cells.workbook) | Copies the theme from another workbook. |
| [`has_exernal_links(self)`](/cells/python-net/aspose.cells/workbook/has_exernal_links/#) | Indicates whether this workbook contains external links to other data sources. |
| [`update_custom_function_definition(self, definition)`](/cells/python-net/aspose.cells/workbook/update_custom_function_definition/#aspose.cells.customfunctiondefinition) | Updates definition of custom functions. |
| [`update_linked_data_source(self, external_workbooks)`](/cells/python-net/aspose.cells/workbook/update_linked_data_source/#list) | If this workbook contains external links to other data source,
| [`set_digital_signature(self, digital_signature_collection)`](/cells/python-net/aspose.cells/workbook/set_digital_signature/#aspose.cells.digitalsignatures.digitalsignaturecollection) | Sets digital signature to an spreadsheet file (Excel2007 and later). |
| [`add_digital_signature(self, digital_signature_collection)`](/cells/python-net/aspose.cells/workbook/add_digital_signature/#aspose.cells.digitalsignatures.digitalsignaturecollection) | Adds digital signature to an OOXML spreadsheet file (Excel2007 and later). |
| [`get_digital_signature(self)`](/cells/python-net/aspose.cells/workbook/get_digital_signature/#) | Gets digital signature from file. |
| [`remove_personal_information(self)`](/cells/python-net/aspose.cells/workbook/remove_personal_information/#) | Removes personal information. |
| [`close(self)`](/cells/python-net/aspose.cells/workbook/close/#) | Dispose() is Skipped by wrapper since  Python protocol |
### Remarks
The Workbook class denotes an Excel spreadsheet. Each spreadsheet can contain multiple worksheets.
The basic feature of the class is to open and save native excel files.
The class has some advanced features like copying data from other Workbooks, combining two Workbooks, converting Excel to PDF, rendering Excel to image and protecting the Excel spreadsheet.
### Example
The following example loads a Workbook from an Excel file named designer.xls and makes the horizontal and vertical scroll bars invisible.
It then replaces two string values with an Integer value and string value respectively within the spreadsheet and finally save the workbook as Excel xlsx file.
```python
from aspose.cells import Workbook
# Open a designer file
designerFile = "designer.xls"
workbook = Workbook(designerFile)
# Set scroll bars
workbook.settings.is_h_scroll_bar_visible = False
workbook.settings.is_v_scroll_bar_visible = False
# Replace the placeholder string with new values
newInt = 100
workbook.replace("OldInt", newInt)
newString = "Hello!"
workbook.replace("OldString", newString)
workbook.save("result.xlsx")
```
### See Also
* module [`aspose.cells`](..)
* class [`CellsColor`](/cells/python-net/aspose.cells/cellscolor)
* class [`ContentTypeProperty`](/cells/python-net/aspose.cells.properties/contenttypeproperty)
* class [`DocumentProperty`](/cells/python-net/aspose.cells.properties/documentproperty)
* class [`Style`](/cells/python-net/aspose.cells/style)
* class [`Workbook`](/cells/python-net/aspose.cells/workbook)
* class [`WorksheetCollection`](/cells/python-net/aspose.cells/worksheetcollection)
