---
title: LightCellsDataProvider class
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 1000
url: /python-net/aspose.cells/lightcellsdataprovider/
is_root: false
---

## LightCellsDataProvider class

Represents Data provider for saving large spreadsheet files in light weight mode.



The LightCellsDataProvider type exposes the following members:

### Methods
| Method | Description |
| :- | :- |
| [start_sheet(sheet_index)](/cells/python-net/aspose.cells/lightcellsdataprovider/start_sheet/#int) | Starts to save a worksheet. |
| [next_row()](/cells/python-net/aspose.cells/lightcellsdataprovider/next_row/#) | Gets the next row to be saved. |
| [start_row(row)](/cells/python-net/aspose.cells/lightcellsdataprovider/start_row/#Row) | Starts to save data of one row. |
| [next_cell()](/cells/python-net/aspose.cells/lightcellsdataprovider/next_cell/#) | Gets next cell to be saved. |
| [start_cell(cell)](/cells/python-net/aspose.cells/lightcellsdataprovider/start_cell/#Cell) | Starts to save data of one cell. |
| [is_gather_string()](/cells/python-net/aspose.cells/lightcellsdataprovider/is_gather_string/#) | Checks whether the current string value of cell needs to be gathered into a global pool. |



### Remarks 


When saving a workbook by this mode, [LightCellsDataProvider.start_sheet(sheet_index)](/cells/python-net/aspose.cells/lightcellsdataprovider/start_sheet) will be checked when saving every worksheet in the workbook.
For one sheet, if [LightCellsDataProvider.start_sheet(sheet_index)](/cells/python-net/aspose.cells/lightcellsdataprovider/start_sheet) gives true, then all data and properties of rows/cells of this sheet to be saved
will be provided by the implementation of this interface. In the first place, [LightCellsDataProvider.next_row()](/cells/python-net/aspose.cells/lightcellsdataprovider/next_row) will be called to get the next row index to be saved.
If a valid row index is returned(the row index must be in ascending order for the rows to be saved),
then a Row object representing this row will be provided for implementation to set its properties by [LightCellsDataProvider.start_row(row)](/cells/python-net/aspose.cells/lightcellsdataprovider/start_row).
For one row, [LightCellsDataProvider.next_cell()](/cells/python-net/aspose.cells/lightcellsdataprovider/next_cell) will be checked firstly. If a valid column index be returned(the column index must be in ascending order for all cells of one row to be saved),
then a Cell object representing this cell will be provided for implementation to set its data and properties by [LightCellsDataProvider.start_cell(cell)](/cells/python-net/aspose.cells/lightcellsdataprovider/start_cell).
After data of this cell is set, this cell will be saved directly to the generated spreadsheet file and the next cell will be checked and processed.

### See Also
* module [aspose.cells](..)
