##LightCellsDataHandler class
## LightCellsDataHandler class
Represents cells data handler for reading large spreadsheet files in light weight mode.
The LightCellsDataHandler type exposes the following members:
### Methods
| Method | Description |
| :- | :- |
| [`start_sheet(self, sheet)`](/cells/python-net/aspose.cells/lightcellsdatahandler/start_sheet/#aspose.cells.worksheet) | Starts to process a worksheet. |
| [`start_row(self, row_index)`](/cells/python-net/aspose.cells/lightcellsdatahandler/start_row/#int) | Prepares to process a row. |
| [`process_row(self, row)`](/cells/python-net/aspose.cells/lightcellsdatahandler/process_row/#aspose.cells.row) | Starts to process one row. |
| [`start_cell(self, column_index)`](/cells/python-net/aspose.cells/lightcellsdatahandler/start_cell/#int) | Prepares to process a cell. |
| [`process_cell(self, cell)`](/cells/python-net/aspose.cells/lightcellsdatahandler/process_cell/#aspose.cells.cell) | Starts to process one cell. |
### Remarks
When reading a workbook by this mode, [`LightCellsDataHandler.start_sheet`](/cells/python-net/aspose.cells/lightcellsdatahandler/start_sheet) will be checked when reading every worksheet in the workbook.
For one sheet, if [`LightCellsDataHandler.start_sheet`](/cells/python-net/aspose.cells/lightcellsdatahandler/start_sheet) gives true, then all data and properties of rows/cells of this sheet will be checked
and processed by the implementation of this interface. For every row, [`LightCellsDataHandler.start_row`](/cells/python-net/aspose.cells/lightcellsdatahandler/start_row) will be called to check whether it need to be processed.
If a row needs to be processed, properties of this row will be read firstly and user can access its properties by [`LightCellsDataHandler.process_row`](/cells/python-net/aspose.cells/lightcellsdatahandler/process_row).
if row's cells need to be processed too, then [`LightCellsDataHandler.process_row`](/cells/python-net/aspose.cells/lightcellsdatahandler/process_row) should returns true and then [`LightCellsDataHandler.start_cell`](/cells/python-net/aspose.cells/lightcellsdatahandler/start_cell) will be
called for every existing cell in this row to check whether one cell need to be processed. If one cell needs to be processed,
then [`LightCellsDataHandler.process_cell`](/cells/python-net/aspose.cells/lightcellsdatahandler/process_cell) will be called to process the cell by the implementation of this interface.
Please note, user should only operate on the values and properties of current Row/Cell object provided by corresponding method.
Because the cells data is read from the template file in streaming manner, most of other objects may be reset/update later
after cells data has been loaded. So when user operating other objects in this implementation,
those operations may be not able to affect the objects existing in the workbook. Or even worse, those operations may
cause inconsistent data in the workbook and then cause unpected issue or exception later.
So, for all other objects such as shapes, column width and styles, conditional formattings, ...etc.,
please do not operate them in any methods of this implementation.
Instead, please manage them after the workbook has been constructed.
### See Also
* module [`aspose.cells`](..)
