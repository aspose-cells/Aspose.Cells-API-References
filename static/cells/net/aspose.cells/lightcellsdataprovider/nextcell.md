##LightCellsDataProvider.NextCell
LightCellsDataProvider method. Gets next cell to be saved
## LightCellsDataProvider.NextCell method
Gets next cell to be saved.
```csharp
public int NextCell()
```
### Return Value
column index of the next cell to be saved. -1 means the end of current row data has been reached and no further cell of current row to be saved.
### Remarks
It will be called at the beginning of saving one cell.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class LightCellsDataProviderMethodNextCellDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
workbook.Worksheets.Clear();
var provider = new DemoLightCellsDataProvider();
XlsSaveOptions saveOptions = new XlsSaveOptions { LightCellsDataProvider = provider };
try
{
workbook.Save("NextCellDemo.xlsx", saveOptions);
Console.WriteLine("Workbook saved with LightCellsDataProvider implementation");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
}
private class DemoLightCellsDataProvider : LightCellsDataProvider
{
private int rowIndex = -1;
private int cellIndex = -1;
private readonly object[,] data = new object[2, 2]
{
{ "Column1", "Column2" },
{ 100, 200 }
};
public bool StartSheet(int sheetIndex) => sheetIndex == 0;
public int NextRow()
{
rowIndex++;
cellIndex = -1;
return rowIndex < 2 ? 1 : 0;
}
public void StartRow(Row row) { }
public int NextCell()
{
cellIndex++;
return cellIndex < 2 ? 1 : 0;
}
public void StartCell(Cell cell)
{
cell.PutValue(data[rowIndex, cellIndex]);
}
public bool IsGatherString() => false;
}
}
}
```
### See Also
* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
