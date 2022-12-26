---
title: LightCellsDataHandler class
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 990
url: /python-net/aspose.cells/lightcellsdatahandler/
is_root: false
---

## LightCellsDataHandler class

Represents cells data handler for reading large spreadsheet files in light weight mode.



The LightCellsDataHandler type exposes the following members:

### Methods
| Method | Description |
| :- | :- |
| [start_sheet(sheet)](/cells/python-net/aspose.cells/lightcellsdatahandler/start_sheet/#Worksheet) | Starts to process a worksheet. |
| [start_row(row_index)](/cells/python-net/aspose.cells/lightcellsdatahandler/start_row/#int) | Prepares to process a row. |
| [process_row(row)](/cells/python-net/aspose.cells/lightcellsdatahandler/process_row/#Row) | Starts to process one row. |
| [start_cell(column_index)](/cells/python-net/aspose.cells/lightcellsdatahandler/start_cell/#int) | Prepares to process a cell. |
| [process_cell(cell)](/cells/python-net/aspose.cells/lightcellsdatahandler/process_cell/#Cell) | Starts to process one cell. |


### Remarks 


When reading a workbook by this mode, [LightCellsDataHandler.start_sheet(sheet)](/cells/python-net/aspose.cells/lightcellsdatahandler/start_sheet) will be checked when reading every worksheet in the workbook.
For one sheet, if [LightCellsDataHandler.start_sheet(sheet)](/cells/python-net/aspose.cells/lightcellsdatahandler/start_sheet) gives true, then all data and properties of rows/cells of this sheet will be checked
and processed by the implementation of this interface. For every row, [LightCellsDataHandler.start_row(row_index)](/cells/python-net/aspose.cells/lightcellsdatahandler/start_row) will be called to check whether it need to be processed.
If a row needs to be processed, properties of this row will be read firstly and user can access its properties by [LightCellsDataHandler.process_row(row)](/cells/python-net/aspose.cells/lightcellsdatahandler/process_row).
if row's cells need to be processed too, then [LightCellsDataHandler.process_row(row)](/cells/python-net/aspose.cells/lightcellsdatahandler/process_row) should returns true and then [LightCellsDataHandler.start_cell(column_index)](/cells/python-net/aspose.cells/lightcellsdatahandler/start_cell) will be
called for every existing cell in this row to check whether one cell need to be processed. If one cell needs to be processed,
then [LightCellsDataHandler.process_cell(cell)](/cells/python-net/aspose.cells/lightcellsdatahandler/process_cell) will be called to process the cell by the implementation of this interface.
### See Also

* module [aspose.cells](../)
