##LightCellsDataProvider.StartSheet
LightCellsDataProvider method. Starts to save a worksheet
## LightCellsDataProvider.StartSheet method
Starts to save a worksheet.
```csharp
public bool StartSheet(int sheetIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | Int32 | index of current sheet to be saved. |
### Return Value
true if this provider will provide data for the given sheet; false if given sheet should use its normal data model(Cells).
### Remarks
It will be called at the beginning of saving a worksheet during saving a workbook. If the provider needs to refer to
```csharp
sheetIndex
```
later in startRow(Row) or startCell(Cell) method, that is, if the process needs to know which worksheet is being processed, the implementation should retain the
```csharp
sheetIndex
```
value here.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class LightCellsDataProviderMethodStartSheetWithInt32Demo
{
public static void Run()
{
try
{
Workbook workbook = new Workbook();
workbook.Worksheets.Clear(); // Start with clean worksheet
// Create custom data provider and save with light cells mode
var saveOptions = new OoxmlSaveOptions
{
LightCellsDataProvider = new CustomLightCellsDataProvider()
};
Console.WriteLine("Starting workbook save with LightCellsDataProvider...");
workbook.Save("StartSheetDemoOutput.xlsx", saveOptions);
Console.WriteLine("Workbook saved successfully. Check StartSheetDemoOutput.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing demo: {ex.Message}");
}
}
private class CustomLightCellsDataProvider : LightCellsDataProvider
{
private bool sheetProcessed = false;
// Called when starting to process a worksheet
public bool StartSheet(int sheetIndex)
{
Console.WriteLine($"Processing sheet index: {sheetIndex}");
// Only process first sheet (index 0)
if (sheetIndex == 0)
{
sheetProcessed = true;
return true;
}
return false;
}
public int NextRow()
{
if (sheetProcessed)
{
sheetProcessed = false;
return 0; // Process first row (index 0)
}
return -1; // Stop processing after first row
}
public void StartRow(Row row)
{
row.Height = 20;
}
public int NextCell()
{
return 0; // Process first cell (index 0)
}
public void StartCell(Cell cell)
{
cell.PutValue("Data from LightCellsDataProvider");
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
* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
