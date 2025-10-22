##Interface LightCellsDataProvider
Aspose.Cells.LightCellsDataProvider interface. Represents Data provider for saving large spreadsheet files in light weight mode
## LightCellsDataProvider interface
Represents Data provider for saving large spreadsheet files in light weight mode.
```csharp
public interface LightCellsDataProvider
```
## Methods
| Name | Description |
| --- | --- |
| [IsGatherString](../../aspose.cells/lightcellsdataprovider/isgatherstring/)() | Checks whether the current string value of cell needs to be gathered into a global pool. |
| [NextCell](../../aspose.cells/lightcellsdataprovider/nextcell/)() | Gets next cell to be saved. |
| [NextRow](../../aspose.cells/lightcellsdataprovider/nextrow/)() | Gets the next row to be saved. |
| [StartCell](../../aspose.cells/lightcellsdataprovider/startcell/)(Cell) | Starts to save data of one cell. |
| [StartRow](../../aspose.cells/lightcellsdataprovider/startrow/)(Row) | Starts to save data of one row. |
| [StartSheet](../../aspose.cells/lightcellsdataprovider/startsheet/)(int) | Starts to save a worksheet. |
### Remarks
When saving a workbook by this mode, [`StartSheet`](./startsheet/) will be checked when saving every worksheet in the workbook. For one sheet, if [`StartSheet`](./startsheet/) gives true, then all data and properties to be saved for rows/cells of this sheet will be provided by the implementation of this interface. In the first place, [`NextRow`](./nextrow/) will be called to get the next row index to be saved. If a valid row index is returned(the row index must be in ascending order for the rows to be saved), then a Row object representing this row will be provided by [`StartRow`](./startrow/) for the implementation to set its properties. For one row, [`NextCell`](./nextcell/) will be checked firstly. If a valid column index be returned(the column index must be in ascending order for all cells of current row), then a Cell object representing this cell will be provided by [`StartCell`](./startcell/) for implementation to set its data and properties. After [`StartCell`](./startcell/) the cell will be saved directly to the resultant spreadsheet file. Then the next cell will be checked and processed.  Please note, user should only update values and properties for current Row/Cell object provided by corresponding method. Because the cells data is written to the resultant file in streaming manner, most of other objects may have been written to the resultant file, or have been gathered and written some global data for them. So when user updating other objects while saving cells data, those operations may be not able to affect the saved data. Or even worse, those operations may cause inconsistent data be save to the resultant file and finally make the file corrupted. So, for all other objects such as shapes, column width and styles, conditional formattings, ...etc., please do not operate them in any methods of this implementation. Instead, please manage them and adjust them to the final state before calling "Save" method of the Workbook.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class LightCellsDataProviderDemo
{
public static void LightCellsDataProviderExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a custom LightCellsDataProvider
CustomLightCellsDataProvider dataProvider = new CustomLightCellsDataProvider();
// Set the LightCellsDataProvider for saving the workbook
OoxmlSaveOptions saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsx)
{
LightCellsDataProvider = dataProvider
};
// Save the workbook with the custom LightCellsDataProvider
workbook.Save("LightCellsDataProviderExample.xlsx", saveOptions);
}
}
public class CustomLightCellsDataProvider : LightCellsDataProvider
{
private int currentRow = -1;
private int currentCell = -1;
public bool StartSheet(int sheetIndex)
{
// Start processing the first sheet
return sheetIndex == 0;
}
public int NextRow()
{
// Move to the next row
currentRow++;
currentCell = -1;
// Return the current row index or -1 if no more rows
return currentRow < 10 ? currentRow : -1;
}
public void StartRow(Row row)
{
// Initialize the row if needed
}
public int NextCell()
{
// Move to the next cell
currentCell++;
// Return the current cell index or -1 if no more cells
return currentCell < 10 ? currentCell : -1;
}
public void StartCell(Cell cell)
{
// Set the value of the cell
cell.PutValue($"R{currentRow}C{currentCell}");
}
public bool IsGatherString()
{
// Return whether to gather strings into a global pool
return false;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
