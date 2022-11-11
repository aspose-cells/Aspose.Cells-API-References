---
title: WorksheetCollection
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 1620
url: /cells/python-net/aspose.cells/worksheetcollection/
---

## WorksheetCollection class

Encapsulates a collection of [Worksheet](/cells/python-net/aspose.cells/worksheet/) objects.

The WorksheetCollection type exposes the following members:
## Properties
| Name | Description |
| :- | :- |
|web_extension_task_panes|Gets the list of task panes.|
|web_extensions|Gets the list of task panes.|
|threaded_comment_authors|Gets the list of threaded comment authors.|
|is_refresh_all_connections|Indicates whether refresh all connections on opening file in MS Excel.|
|names|Gets the collection of all the Name objects in the spreadsheet.|
|active_sheet_name|Represents the name of active worksheet when the spreadsheet is opened.|
|active_sheet_index|Represents the index of active worksheet when the spreadsheet is opened.|
|dxfs|Gets the master differential formatting records.|
|xml_maps|Gets and sets the XML maps in the workbook.|
|built_in_document_properties|Returns a [DocumentProperty](/cells/python-net/aspose.cells.properties/documentproperty/) collection that represents all the built-in document properties of the spreadsheet.|
|custom_document_properties|Returns a [DocumentProperty](/cells/python-net/aspose.cells.properties/documentproperty/) collection that represents all the custom document properties of the spreadsheet.|
|ole_size|Gets and Sets displayed size when Workbook file is used as an Ole object.|
|external_links|Represents external links in a workbook.|
|table_styles|Gets [table_styles](/cells/python-net/aspose.cells/worksheetcollection/) object.|
|revision_logs|Represents revision logs.|
|capacity|  |
## Methods
| Name | Description |
| :- | :- |
|get(index)|Add API for Python Via .Net.since this[int index] is unsupported|
|get(sheet_name)|Add API for Python Via .Net.since this[string sheetName] is unsupported|
|add(type)|Adds a worksheet to the collection.|
|add()|Adds a worksheet to the collection.|
|add(sheet_name)|Adds a worksheet to the collection.|
|register_add_in_function(add_in_file, function_name, lib)|Adds addin function into the workbook|
|register_add_in_function(id, function_name)|Adds addin function into the workbook|
|add_copy(sheet_name)|Adds a worksheet to the collection and copies data from an existed worksheet.|
|add_copy(sheet_index)|Adds a worksheet to the collection and copies data from an existed worksheet.|
|get_range_by_name(range_name)|Gets Range object by pre-defined name.|
|get_range_by_name(range_name, current_sheet_index, include_table)|Gets [Range](/cells/python-net/aspose.cells/range/) by pre-defined name or table's name|
|copy_to(array)|  |
|copy_to(index, array, array_index, count)|  |
|index_of(item, index)|  |
|index_of(item, index, count)|  |
|last_index_of(item)|  |
|last_index_of(item, index)|  |
|last_index_of(item, index, count)|  |
|create_range(address, sheet_index)|Creates a [Range](/cells/python-net/aspose.cells/range/) object from an address of the range.|
|create_union_range(address, sheet_index)|Creates a [Range](/cells/python-net/aspose.cells/range/) object from an address of the range.|
|get_sheet_by_code_name(code_name)|Gets the worksheet by the code name.|
|sort_names()|Sorts the defined names.|
|swap_sheet(sheet_index1, sheet_index2)|Swaps the two sheets.|
|remove_at(name)|Removes the element at a specified name.|
|get_named_ranges()|Gets all pre-defined named ranges in the spreadsheet.|
|get_named_ranges_and_tables()|Gets all pre-defined named ranges in the spreadsheet.|
|set_ole_size(start_row, end_row, start_column, end_column)|Sets displayed size when Workbook file is used as an Ole object.|
|clear_pivottables()|Clears pivot tables from the spreadsheet.|
|refresh_pivot_tables()|Refreshes all the PivotTables in the WorksheetCollection.|
|binary_search(item)|  |

### See Also

* namespace [aspose.cells](/cells/python-net/aspose.cells/)
* assembly [Aspose.Cells](/cells/python-net/)

