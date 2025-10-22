##LightCellsDataProvider.IsGatherString
LightCellsDataProvider method. Checks whether the current string value of cell needs to be gathered into a global pool
## LightCellsDataProvider.IsGatherString method
Checks whether the current string value of cell needs to be gathered into a global pool.
```csharp
public bool IsGatherString()
```
### Return Value
true if string value need to be gathered into a global pool for the resultant file.
### Remarks
Gathering string values will take advantage only when there are many duplicated string values for the cells provided by this implementation. In this situation gathering string will save much memory and generate smaller resultant file. If there are many string values for the cells provided by LightCellsDataProvider but few of them are same, gathering string will cost more memory and time and has no advantage for the resultant file.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class LightCellsDataProviderMethodIsGatherStringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
workbook.Worksheets.Clear();
var saveOptions = new OoxmlSaveOptions
{
LightCellsDataProvider = new CustomLightCellsDataProvider()
};
try
{
workbook.Save("IsGatherStringDemo.xlsx", saveOptions);
Console.WriteLine("Workbook saved with IsGatherString implementation");
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
private readonly object[,] data = new object[3, 2]
{
{ "Product", "Price" },
{ "Laptop", 1200.50 },
{ "Phone", 899.99 }
};
public bool StartSheet(int sheetIndex)
{
return sheetIndex == 0;
}
public int NextRow()
{
rowIndex++;
cellIndex = -1;
return rowIndex < 3 ? rowIndex : -1;
}
public void StartRow(Row row)
{
row.Height = 15;
}
public int NextCell()
{
cellIndex++;
return cellIndex < 2 ? cellIndex : -1;
}
public void StartCell(Cell cell)
{
cell.PutValue(data[rowIndex, cellIndex]);
}
public bool IsGatherString()
{
// Only gather strings for header row (rowIndex 0)
return rowIndex == 0;
}
}
}
}
```
### See Also
* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
