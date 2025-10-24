##LightCellsDataProvider.NextRow
LightCellsDataProvider method. Gets the next row to be saved
## LightCellsDataProvider.NextRow method
Gets the next row to be saved.
```csharp
public int NextRow()
```
### Return Value
the next row index to be saved. -1 means the end of current sheet data has been reached and no further row of current sheet to be saved.
### Remarks
It will be called at the beginning of saving a row and its cells data(before [`StartRow`](../startrow/)).
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class LightCellsDataProviderMethodNextRowDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
workbook.Worksheets.Clear();
workbook.Worksheets.Add("Sheet1");
OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
saveOptions.LightCellsDataProvider = new CustomLightCellsDataProvider();
try
{
workbook.Save("LightCellsDataProviderMethodNextRowDemo.xlsx", saveOptions);
Console.WriteLine("Workbook saved with LightCellsDataProvider implementation.");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
}
}
public class CustomLightCellsDataProvider : LightCellsDataProvider
{
private int currentRow = -1;
private int currentCell = -1;
private readonly int totalRows = 3;
public bool StartSheet(int sheetIndex)
{
return sheetIndex == 0;
}
public int NextRow()
{
currentRow++;
currentCell = -1;
return currentRow < totalRows ? currentRow : -1;
}
public void StartRow(Row row)
{
row.Height = 20;
}
public int NextCell()
{
currentCell++;
return currentCell < 2 ? currentCell : -1;
}
public void StartCell(Cell cell)
{
cell.PutValue($"R{currentRow}C{currentCell}");
}
public bool IsGatherString()
{
return false;
}
}
}
```
### See Also
* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
