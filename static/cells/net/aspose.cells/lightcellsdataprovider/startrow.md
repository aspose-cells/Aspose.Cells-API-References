##LightCellsDataProvider.StartRow
LightCellsDataProvider method. Starts to save data of one row
## LightCellsDataProvider.StartRow method
Starts to save data of one row.
```csharp
public void StartRow(Row row)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Row | Row object for implementation to fill data. Its row index is the returned value of latest call of [`NextRow`](../nextrow/). If the row has been initialized in the inner cells model, the existing row object will be used. Otherwise a temporary Row object will be used for implementation to fill data. |
### Remarks
It will be called at the beginning of saving a row and its cells data. If current row has some custom properties such as height, style, ...etc., implementation should set those properties to given Row object here.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class LightCellsDataProviderMethodStartRowWithRowDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a custom data provider
var saveOptions = new OoxmlSaveOptions
{
LightCellsDataProvider = new CustomLightCellsDataProvider()
};
try
{
// Process the workbook with our custom data provider
workbook.Save("StartRowDemo.xlsx", saveOptions);
Console.WriteLine("Workbook processed successfully with StartRow implementation.");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing StartRow method: {ex.Message}");
}
}
private class CustomLightCellsDataProvider : LightCellsDataProvider
{
private int currentRow = -1;
private readonly int totalRows = 5;
public bool StartSheet(int sheetIndex)
{
return sheetIndex == 0;
}
public int NextRow()
{
currentRow++;
return currentRow < totalRows ? currentRow : -1;
}
public void StartRow(Row row)
{
// Demonstrate StartRow method with Row parameter
row.Height = 25;
row.IsHidden = (currentRow % 2 == 0);
Console.WriteLine($"Processing row {row.Index}, Height: {row.Height}, Hidden: {row.IsHidden}");
}
public int NextCell()
{
return 0; // Process only first cell in each row
}
public void StartCell(Cell cell)
{
cell.PutValue($"Row {cell.Row + 1} Data");
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
* class [Row](../../row/)
* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
