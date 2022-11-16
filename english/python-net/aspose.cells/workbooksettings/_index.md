---
title: WorkbookSettings
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 1600
url: /python-net/aspose.cells/workbooksettings/
---

## WorkbookSettings class

Represents all settings of the workbook.

The WorkbookSettings type exposes the following members:
## Properties
| Name | Description |
| :- | :- |
|stream_provider|Gets and sets the stream provider for external resource.|
|resource_provider|Gets and sets the stream provider for external resource, such as loading image data for picture of type "LinkToFile".|
|author|Gets and sets the author of the file.|
|check_custom_number_format|Indicates whether checking custom number format when setting Style.Custom.|
|enable_macros|Enable macros;|
|date1904|Gets or sets a value which represents if the workbook uses the 1904 date system.|
|protection_type|Gets the protection type of the workbook.|
|display_drawing_objects|Indicates whether and how to show objects in the workbook.|
|sheet_tab_bar_width|Width of worksheet tab bar (in 1/1000 of window width).|
|show_tabs|Get or sets a value whether the Workbook tabs are displayed.|
|first_visible_tab|Gets or sets the first visible worksheet tab.|
|is_h_scroll_bar_visible|Gets or sets a value indicating whether the generated spreadsheet will contain a horizontal scroll bar.|
|is_v_scroll_bar_visible|Gets or sets a value indicating whether the generated spreadsheet will contain a vertical scroll bar.|
|shared|Gets or sets a value that indicates whether the Workbook is shared.|
|language_code|Gets or sets the user interface language of the Workbook version based on CountryCode that has saved the file.|
|region|Gets or sets the regional settings for workbook.|
|globalization_settings|Gets and sets the globalization settings.|
|number_decimal_separator|Gets or sets the decimal separator for formatting/parsing numeric values. Default is the decimal separator of current Region.|
|number_group_separator|Gets or sets the character that separates groups of digits to the left of the decimal in numeric values. Default is the group separator of current Region.|
|password|Represents Workbook file encryption password.|
|write_protection|Provides access to the workbook write protection options.|
|is_encrypted|Gets a value that indicates whether a password is required to open this workbook.|
|is_protected|Gets a value that indicates whether the structure or window of the Workbook is protected.|
|is_default_encrypted|Indicates whether encrypting the workbook with default password if Structure and Windows of the workbook are locked.|
|is_minimized|Represents whether the generated spreadsheet will be opened Minimized.|
|is_hidden|Indicates whether this workbook is hidden.|
|auto_compress_pictures|Specifies a boolean value that indicates the application automatically compressed pictures in the workbook.|
|remove_personal_information|True if personal information can be removed from the specified workbook.|
|hide_pivot_field_list|Gets and sets whether hide the field list for the PivotTable.|
|update_links_type|Gets and sets how updates external links when the workbook is opened.|
|max_row|Gets the max row index, zero-based.|
|max_column|Gets the max column index, zero-based.|
|parsing_formula_on_open|Indicates whether parsing the formula when reading the file.|
|window_left|The distance from the left edge of the client area to the left edge of the window, in unit of point.|
|window_left_inch|The distance from the left edge of the client area to the left edge of the window.<br/>            In unit of inch.|
|window_left_cm|The distance from the left edge of the client area to the left edge of the window.<br/>            In unit of centimeter.|
|window_top|The distance from the top edge of the client area to the top edge of the window, in unit of point.|
|window_top_inch|The distance from the top edge of the client area to the top edge of the window, in unit of inch.|
|window_top_cm|The distance from the top edge of the client area to the top edge of the window, in unit of centimeter.|
|window_width|The width of the window, in unit of point.|
|window_width_inch|The width of the window, in unit of inch.|
|window_width_cm|The width of the window, in unit of centimeter.|
|window_height|The height of the window, in unit of point.|
|window_height_inch|The height of the window, in unit of inch.|
|window_height_cm|The height of the window, in unit of centimeter.|
|update_adjacent_cells_border|Indicates whether update adjacent cells' border.|
|significant_digits|Gets and sets the number of significant digits.<br/>            The default value is [significant_digits](/cells/python-net/aspose.cells/cellshelper/).|
|check_compatibility|Indicates whether check compatibility with earlier versions when saving workbook.|
|check_excel_restriction|Whether check restriction of excel file when user modify cells related objects.<br/>            For example, excel does not allow inputting string value longer than 32K.<br/>            When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception.<br/>            If this property is false, we will accept your input string value as the cell's value so that later<br/>            you can output the complete string value for other file formats such as CSV.<br/>            However, if you have set such kind of value that is invalid for excel file format,<br/>            you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file.|
|auto_recover|Indicates whether the file is mark for auto-recovery.|
|crash_save|indicates whether the application last saved the workbook file after a crash.|
|data_extract_load|indicates whether the application last opened the workbook for data recovery.|
|repair_load|Indicates whether the application last opened the workbook in safe or repair mode.|
|build_version|Specifies the incremental public release of the application.|
|memory_setting|Gets or sets the memory usage options. The new option will be taken as the default option for newly created worksheets but does not take effect for existing worksheets.|
|paper_size|Gets and sets the default print paper size.|
|warning_callback|Gets or sets warning callback.|
|max_rows_of_shared_formula|Gets and sets the max row number of shared formula.|
|compliance|Specifies the OOXML version for the output document. The default value is Ecma376_2006.|
|quote_prefix_to_style|Indicates whether setting [quote_prefix](/cells/python-net/aspose.cells/style/) property when entering the string value(which starts  with single quote mark ) to the cell|
|formula_settings|Gets the settings for formula-related features.|
|precision_as_displayed|True if calculations in this workbook will be done using only the precision of the numbers as they're displayed|
|re_calculate_on_open|Indicates whether re-calculate all formulas on opening file.|
|create_calc_chain|Whether creates calculated formulas chain. Default is false.|
|force_full_calculate|Fully calculates every time when a calculation is triggered.|
|iteration|Indicates whether enable iterative calculation to resolve circular references.|
|max_iteration|Returns or sets the maximum number of iterations to resolve a circular reference.|
|max_change|Returns or sets the maximum number of change to resolve a circular reference.|
|calc_mode|It specifies whether to calculate formulas manually,<br/>            automatically or automatically except for multiple table operations.|
|calculation_id|Specifies the version of the calculation engine used to calculate values in the workbook.|
|calc_stack_size|Specifies the stack size for calculating cells recursively.<br/>            The large value for this size will give better performance when there are lots of cells need to be calculated recursively.<br/>            On the other hand, larger value will raise the risk of StackOverflowException.<br/>            If user gets StackOverflowException when calculating formulas, this value should be decreased.|
|recalculate_before_save|Indicates whether to recalculate before saving the document.|
## Methods
| Name | Description |
| :- | :- |
|get_theme_font(type)|Gets the default theme font name.|
|set_page_orientation_type(page_orientation_type)|Set the type of  print orientation for the whole workbook.|

### See Also

* namespace [aspose.cells](/cells/python-net/aspose.cells/)
* assembly [Aspose.Cells](/cells/python-net/)

