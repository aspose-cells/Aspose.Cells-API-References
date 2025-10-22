##LightCellsDataProvider class
## LightCellsDataProvider class
Represents Data provider for saving large spreadsheet files in light weight mode.
The LightCellsDataProvider type exposes the following members:
### Methods
| Method | Description |
| :- | :- |
| [`start_sheet(self, sheet_index)`](/cells/python-net/aspose.cells/lightcellsdataprovider/start_sheet/#int) | Starts to save a worksheet. |
| [`next_row(self)`](/cells/python-net/aspose.cells/lightcellsdataprovider/next_row/#) | Gets the next row to be saved. |
| [`start_row(self, row)`](/cells/python-net/aspose.cells/lightcellsdataprovider/start_row/#aspose.cells.row) | Starts to save data of one row. |
| [`next_cell(self)`](/cells/python-net/aspose.cells/lightcellsdataprovider/next_cell/#) | Gets next cell to be saved. |
| [`start_cell(self, cell)`](/cells/python-net/aspose.cells/lightcellsdataprovider/start_cell/#aspose.cells.cell) | Starts to save data of one cell. |
| [`is_gather_string(self)`](/cells/python-net/aspose.cells/lightcellsdataprovider/is_gather_string/#) | Checks whether the current string value of cell needs to be gathered into a global pool. |
### Remarks
When saving a workbook by this mode, [`LightCellsDataProvider.start_sheet`](/cells/python-net/aspose.cells/lightcellsdataprovider/start_sheet) will be checked when saving every worksheet in the workbook.
For one sheet, if [`LightCellsDataProvider.start_sheet`](/cells/python-net/aspose.cells/lightcellsdataprovider/start_sheet) gives true, then all data and properties to be saved for rows/cells of this sheet
will be provided by the implementation of this interface.
In the first place, [`LightCellsDataProvider.next_row`](/cells/python-net/aspose.cells/lightcellsdataprovider/next_row) will be called to get the next row index to be saved.
If a valid row index is returned(the row index must be in ascending order for the rows to be saved),
then a Row object representing this row will be provided by [`LightCellsDataProvider.start_row`](/cells/python-net/aspose.cells/lightcellsdataprovider/start_row) for the implementation to set its properties.
For one row, [`LightCellsDataProvider.next_cell`](/cells/python-net/aspose.cells/lightcellsdataprovider/next_cell) will be checked firstly.
If a valid column index be returned(the column index must be in ascending order for all cells of current row),
then a Cell object representing this cell will be provided by [`LightCellsDataProvider.start_cell`](/cells/python-net/aspose.cells/lightcellsdataprovider/start_cell) for implementation to set its data and properties.
After [`LightCellsDataProvider.start_cell`](/cells/python-net/aspose.cells/lightcellsdataprovider/start_cell) the cell will be saved directly to the resultant spreadsheet file.
Then the next cell will be checked and processed.
Please note, user should only update values and properties for current Row/Cell object provided by corresponding method.
Because the cells data is written to the resultant file in streaming manner, most of other objects may have been written
to the resultant file, or have been gathered and written some global data for them. So when user updating other objects
while saving cells data, those operations may be not able to affect the saved data. Or even worse, those operations may
cause inconsistent data be save to the resultant file and finally make the file corrupted.
So, for all other objects such as shapes, column width and styles, conditional formattings, ...etc.,
please do not operate them in any methods of this implementation.
Instead, please manage them and adjust them to the final state before calling "Save" method of the Workbook.
### See Also
* module [`aspose.cells`](..)
