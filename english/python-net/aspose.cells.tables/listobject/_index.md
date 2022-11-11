---
title: ListObject
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 30
url: /python-net/aspose.cells.tables/listobject/
---

## ListObject class

Represents a list object on a worksheet.<br/>            The ListObject object is a member of the ListObjects collection. <br/>            The ListObjects collection contains all the list objects on a worksheet.

The ListObject type exposes the following members:
## Properties
| Name | Description |
| :- | :- |
|start_row|Gets the start row of the range.|
|start_column|Gets the start column of the range.|
|end_row|Gets the end  row of the range.|
|end_column|Gets the end column of the range.|
|list_columns|Gets ListColumns of the ListObject.|
|show_header_row|Gets and sets whether this ListObject show header row.|
|show_totals|Gets and sets whether this ListObject show total row.|
|data_range|Gets the data range of the ListObject.|
|query_table|Gets the linked QueryTable.|
|data_source_type|Gets the data source type of the table.|
|auto_filter|Gets auto filter.|
|display_name|Gets and sets the display name.|
|comment|Gets and sets the comment of the table.|
|show_table_style_first_column|Indicates whether the first column in the table should have the style applied.|
|show_table_style_last_column|Indicates whether the last column in the table should have the style applied.|
|show_table_style_row_stripes|Indicates whether row stripe formatting is applied.|
|show_table_style_column_stripes|Indicates whether column stripe formatting is applied.|
|table_style_type|Gets and the built-in table style.|
|table_style_name|Gets and sets the table style name.|
|xml_map|Gets an [xml_map](/python-net/aspose.cells.tables/listobject/) used for this list.|
|alternative_text|Gets and sets the alternative text.|
|alternative_description|Gets and sets the alternative description.|
## Methods
| Name | Description |
| :- | :- |
|convert_to_range()|Convert the table to range.|
|convert_to_range(options)|Convert the table to range.|
|resize(start_row, start_column, end_row, end_column, has_headers)|Resize the range of the list object.|
|put_cell_value(row_offset, column_offset, value)|Put the value to the cell.|
|update_column_name()|Updates all list columns' name from the worksheet.|
|filter()|Filter the table.|
|apply_style_to_range()|Apply the table style to the range.|

### See Also

* namespace [aspose.cells.tables](/python-net/aspose.cells.tables/)
* assembly [Aspose.Cells](/python-net/)

