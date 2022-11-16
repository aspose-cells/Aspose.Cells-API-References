---
title: Workbook
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 1580
url: /cells/python-net/aspose.cells/workbook/
---

## Workbook class

Represents a root object to create an Excel spreadsheet.

The Workbook type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|Workbook()|Initializes a new instance of the [Workbook](/cells/python-net/aspose.cells/workbook/) class.|
|Workbook(file_format_type)|Initializes a new instance of the Workbook class|
|Workbook(file)|Initializes a new instance of the Workbook class|
|Workbook(stream)|Initializes a new instance of the Workbook class|
|Workbook(file, load_options)|Initializes a new instance of the Workbook class|
|Workbook(stream, load_options)|Initializes a new instance of the Workbook class|
## Properties
| Name | Description |
| :- | :- |
|settings|Represents the workbook settings.|
|worksheets|Gets the [WorksheetCollection](/cells/python-net/aspose.cells/worksheetcollection/) collection in the spreadsheet.|
|is_licensed|Indicates whether license is set.|
|colors|Returns colors in the palette for the spreadsheet.|
|count_of_styles_in_pool|Gets number of the styles in the style pool.|
|default_style|Gets or sets the default [Style](/cells/python-net/aspose.cells/style/) object of the workbook.|
|is_digitally_signed|Indicates if this spreadsheet is digitally signed.|
|is_workbook_protected_with_password|Indicates whether structure or window is protected with password.|
|vba_project|Gets the [vba_project](/cells/python-net/aspose.cells/workbook/) in a spreadsheet.|
|has_macro|Indicates if this spreadsheet contains macro/VBA.|
|has_revisions|Gets if the workbook has any tracked changes|
|file_name|Gets and sets the current file name.|
|cells_data_table_factory|Gets the factory for building ICellsDataTable from custom objects|
|data_sorter|Gets a DataSorter object to sort data.|
|theme|Gets the theme name.|
|built_in_document_properties|Returns a [DocumentProperty](/cells/python-net/aspose.cells.properties/documentproperty/) collection that represents all the built-in document properties of the spreadsheet.|
|custom_document_properties|Returns a [DocumentProperty](/cells/python-net/aspose.cells.properties/documentproperty/) collection that represents all the custom document properties of the spreadsheet.|
|file_format|Gets and sets the file format.|
|interrupt_monitor|Gets and sets the interrupt monitor.|
|content_type_properties|Gets the list of  [ContentTypeProperty](/cells/python-net/aspose.cells.properties/contenttypeproperty/) objects in the workbook.|
|custom_xml_parts|Represents a Custom XML Data Storage Part (custom XML data within a package).|
|data_mashup|Gets mashup data.|
|ribbon_xml|Gets and sets the XML file that defines the Ribbon UI.|
|absolute_path|Gets and sets the absolute path of the file.|
|data_connections|Gets the [ExternalConnection](/cells/python-net/aspose.cells.externalconnections/externalconnection/) collection.|
## Methods
| Name | Description |
| :- | :- |
|save(file_name, save_format)|Saves the workbook to the disk.|
|save(file_name)|Saves the workbook to the disk.|
|save(file_name, save_options)|Saves the workbook to the disk.|
|save(stream, save_format)|Saves the workbook to the stream.|
|save(stream, save_options)|Saves the workbook to the stream.|
|replace(place_holder, new_value)|Replaces a cell's value with a new string.|
|replace(place_holder, new_value)|Replaces a cell's value with a new integer.|
|replace(place_holder, new_value)|Replaces a cell's value with a new double.|
|replace(place_holder, new_values, is_vertical)|Replaces a cell's value with a new string array.|
|replace(place_holder, new_values, is_vertical)|Replaces cells' values with an integer array.|
|replace(place_holder, new_values, is_vertical)|Replaces cells' values with a double array.|
|replace(bool_value, new_value)|Replaces cells' values with new data.|
|replace(int_value, new_value)|Replaces cells' values with new data.|
|replace(place_holder, new_value, options)|Replaces a cell's value with a new string.|
|copy(source, copy_options)|Copies data from a source Workbook object.|
|copy(source)|Copies data from a source Workbook object.|
|calculate_formula()|Calculates the result of formulas.|
|calculate_formula(ignore_error)|Calculates the result of formulas.|
|calculate_formula(ignore_error, custom_function)|Calculates the result of formulas.|
|calculate_formula(options)|Calculating formulas in this workbook.|
|refresh_dynamic_array_formulas(calculate)|Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data)<br/>            Other formulas in the workbook will not be calculated recursively even if they were used by dynamic array formulas.|
|refresh_dynamic_array_formulas(calculate, copts)|Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data)|
|import_xml(url, sheet_name, row, col)|Imports/Updates an XML data file into the workbook.|
|import_xml(stream, sheet_name, row, col)|Imports/Updates an XML data file into the workbook.|
|export_xml(map_name, path)|Export XML data linked by the specified XML map.|
|export_xml(map_name, stream)|Export XML data.|
|parse_formulas(ignore_error)|Parses all formulas which have not been parsed when they were loaded from template file or set to a cell.|
|start_access_cache(opts)|Starts the session that uses caches to access data.|
|close_access_cache(opts)|Closes the session that uses caches to access data.|
|remove_unused_styles()|Remove all unused styles.|
|create_style()|Creates a new style.|
|create_builtin_style(type)|Creates built-in style by given type.|
|create_cells_color()|Creates a [CellsColor](/cells/python-net/aspose.cells/cellscolor/) object.|
|combine(second_workbook)|Combines another Workbook object.|
|get_style_in_pool(index)|Gets the style in the style pool.<br/>            All styles in the workbook will be gathered into a pool.<br/>            There is only a simple reference index in the cells.|
|get_fonts()|Gets all fonts in the style pool.|
|get_named_style(name)|Gets the named style in the style pool.|
|change_palette(color, index)|Changes the palette for the spreadsheet in the specified index.|
|is_color_in_palette(color)|Checks if a color is in the palette for the spreadsheet.|
|get_matching_color(raw_color)|Find best matching Color in current palette.|
|set_encryption_options(encryption_type, key_length)|Set Encryption Options.|
|protect(protection_type, password)|Protects a workbook.|
|protect_shared_workbook(password)|Protects a shared workbook.|
|unprotect(password)|Unprotects a workbook.|
|unprotect_shared_workbook(password)|Unprotects a shared workbook.|
|remove_macro()|Removes VBA/macro from this spreadsheet.|
|remove_digital_signature()|Removes digital signature from this spreadsheet.|
|accept_all_revisions()|Accepts all tracked changes in the workbook.|
|remove_external_links()|Removes all external links in the workbook.|
|get_theme_color(type)|Gets theme color.|
|set_theme_color(type, color)|Sets the theme color|
|custom_theme(theme_name, colors)|Customs the theme.|
|copy_theme(source)|Copies the theme from another workbook.|
|has_exernal_links()|Indicates whether this workbook contains external links to other data sources.|
|update_linked_data_source(external_workbooks)|If this workbook contains external links to other data source,<br/>            Aspose.Cells will attempt to retrieve the latest data.|
|set_digital_signature(digital_signature_collection)|Sets digital signature to an spreadsheet file (Excel2007 and later).|
|add_digital_signature(digital_signature_collection)|Adds digital signature to an OOXML spreadsheet file (Excel2007 and later).|
|get_digital_signature()|Gets digital signature from file.|
|remove_personal_information()|Removes personal information.|

### See Also

* namespace [aspose.cells](/cells/python-net/aspose.cells/)
* assembly [Aspose.Cells](/cells/python-net/)

