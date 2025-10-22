##Aspose::Cells::LightCellsDataHandler class
'Aspose::Cells::LightCellsDataHandler class. Represents cells data handler for reading large spreadsheet files in light weight mode in C++.'
## LightCellsDataHandler class
Represents cells data handler for reading large spreadsheet files in light weight mode.
```cpp
class LightCellsDataHandler
```
## Methods
| Method | Description |
| --- | --- |
| virtual [ProcessCell(Cell\& cell)](./processcell/) | Starts to process one cell. |
| virtual [ProcessRow(Row\& row)](./processrow/) | Starts to process one row. |
| virtual [StartCell(int32_t columnIndex)](./startcell/) | Prepares to process a cell. |
| virtual [StartRow(int32_t rowIndex)](./startrow/) | Prepares to process a row. |
| virtual [StartSheet(Worksheet\& sheet)](./startsheet/) | Starts to process a worksheet. |
## Remarks
When reading a workbook by this mode, StartSheet(Worksheet) will be checked when reading every worksheet in the workbook. For one sheet, if StartSheet(Worksheet) gives true, then all data and properties of rows/cells of this sheet will be checked and processed by the implementation of this interface. For every row, [StartRow(int)](./startrow/) will be called to check whether it need to be processed. If a row needs to be processed, properties of this row will be read firstly and user can access its properties by ProcessRow(Row). if row's cells need to be processed too, then ProcessRow(Row) should returns true and then [StartCell(int)](./startcell/) will be called for every existing cell in this row to check whether one cell need to be processed. If one cell needs to be processed, then ProcessCell(Cell) will be called to process the cell by the implementation of this interface.
Please note, user should only operate on the values and properties of current Row/Cell object provided by corresponding method. Because the cells data is read from the template file in streaming manner, most of other objects may be reset/update later after cells data has been loaded. So when user operating other objects in this implementation, those operations may be not able to affect the objects existing in the workbook. Or even worse, those operations may cause inconsistent data in the workbook and then cause unpected issue or exception later. So, for all other objects such as shapes, column width and styles, conditional formattings, ...etc., please do not operate them in any methods of this implementation. Instead, please manage them after the workbook has been constructed.
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
