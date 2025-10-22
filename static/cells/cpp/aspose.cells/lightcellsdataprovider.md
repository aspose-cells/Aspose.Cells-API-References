##Aspose::Cells::LightCellsDataProvider class
'Aspose::Cells::LightCellsDataProvider class. Represents Data provider for saving large spreadsheet files in light weight mode in C++.'
## LightCellsDataProvider class
Represents Data provider for saving large spreadsheet files in light weight mode.
```cpp
class LightCellsDataProvider
```
## Methods
| Method | Description |
| --- | --- |
| virtual [IsGatherString()](./isgatherstring/) | Checks whether the current string value of cell needs to be gathered into a global pool. |
| virtual [NextCell()](./nextcell/) | Gets next cell to be saved. |
| virtual [NextRow()](./nextrow/) | Gets the next row to be saved. |
| virtual [StartCell(Cell\& cell)](./startcell/) | Starts to save data of one cell. |
| virtual [StartRow(Row\& row)](./startrow/) | Starts to save data of one row. |
| virtual [StartSheet(int32_t sheetIndex)](./startsheet/) | Starts to save a worksheet. |
## Remarks
When saving a workbook by this mode, [StartSheet(int)](./startsheet/) will be checked when saving every worksheet in the workbook. For one sheet, if [StartSheet(int)](./startsheet/) gives true, then all data and properties to be saved for rows/cells of this sheet will be provided by the implementation of this interface. In the first place, [NextRow()](./nextrow/) will be called to get the next row index to be saved. If a valid row index is returned(the row index must be in ascending order for the rows to be saved), then a [Row](../row/) object representing this row will be provided by StartRow(Row) for the implementation to set its properties. For one row, [NextCell()](./nextcell/) will be checked firstly. If a valid column index be returned(the column index must be in ascending order for all cells of current row), then a [Cell](../cell/) object representing this cell will be provided by StartCell(Cell) for implementation to set its data and properties. After StartCell(Cell) the cell will be saved directly to the resultant spreadsheet file. Then the next cell will be checked and processed.
Please note, user should only update values and properties for current Row/Cell object provided by corresponding method. Because the cells data is written to the resultant file in streaming manner, most of other objects may have been written to the resultant file, or have been gathered and written some global data for them. So when user updating other objects while saving cells data, those operations may be not able to affect the saved data. Or even worse, those operations may cause inconsistent data be save to the resultant file and finally make the file corrupted. So, for all other objects such as shapes, column width and styles, conditional formattings, ...etc., please do not operate them in any methods of this implementation. Instead, please manage them and adjust them to the final state before calling "Save" method of the [Workbook](../workbook/).
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
