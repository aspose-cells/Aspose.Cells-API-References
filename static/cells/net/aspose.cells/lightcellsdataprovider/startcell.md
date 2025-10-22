##LightCellsDataProvider.StartCell
LightCellsDataProvider method. Starts to save data of one cell
## LightCellsDataProvider.StartCell method
Starts to save data of one cell.
```csharp
public void StartCell(Cell cell)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cell | Cell | Cell object for implementation to fill data. Its column index is the returned value of latest call of [`NextCell`](../nextcell/). If the cell has been initialized in the inner cells model, the existed cell object will be used. Otherwise a temporary Cell object will be used for implementation to fill data. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class LightCellsDataProviderMethodStartCellWithCellDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a cell to use as parameter
Cell cell = worksheet.Cells["A1"];
cell.PutValue("Sample Data");
// Create custom data provider
var saveOptions = new OoxmlSaveOptions
{
LightCellsDataProvider = new CustomLightCellsDataProvider()
};
try
{
workbook.Save("StartCellWithCellDemo.xlsx", saveOptions);
Console.WriteLine("Workbook saved with StartCell implementation");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
}
private class CustomLightCellsDataProvider : LightCellsDataProvider
{
private int rowIndex = -1;
private int cellIndex = -1;
private readonly int totalRows = 5;
private readonly int totalCells = 3;
public bool StartSheet(int sheetIndex)
{
return sheetIndex == 0;
}
public int NextRow()
{
rowIndex++;
cellIndex = -1;
return rowIndex < totalRows ? rowIndex : -1;
}
public void StartRow(Row row)
{
row.Height = 15;
}
public int NextCell()
{
cellIndex++;
return cellIndex < totalCells ? cellIndex : -1;
}
public void StartCell(Cell cell)
{
cell.PutValue($"Row {cell.Row + 1}, Col {cell.Column + 1}");
}
public bool IsGatherString()
{
return false;
}
}
}
}
```
### See Also
* class [Cell](../../cell/)
* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
