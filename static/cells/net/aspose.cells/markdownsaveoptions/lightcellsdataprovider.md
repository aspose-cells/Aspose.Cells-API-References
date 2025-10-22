##MarkdownSaveOptions.LightCellsDataProvider
MarkdownSaveOptions property. The Data provider to provide cells data for saving workbook in light mode
## MarkdownSaveOptions.LightCellsDataProvider property
The Data provider to provide cells data for saving workbook in light mode.
```csharp
public LightCellsDataProvider LightCellsDataProvider { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Collections.Generic;
public class MarkdownSaveOptionsPropertyLightCellsDataProviderDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate some sample data
for (int i = 0; i < 10; i++)
{
worksheet.Cells[i, 0].Value = "Item " + (i + 1);
worksheet.Cells[i, 1].Value = i + 1;
}
// Create custom LightCellsDataProvider
var dataProvider = new CustomLightCellsDataProvider();
// Create MarkdownSaveOptions
MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
// Display current value (should be null initially)
Console.WriteLine("Current LightCellsDataProvider value: " + (saveOptions.LightCellsDataProvider == null ? "null" : "set"));
// Set the custom data provider
saveOptions.LightCellsDataProvider = dataProvider;
// Save with the custom data provider
workbook.Save("LightCellsDataProviderDemo.md", saveOptions);
}
}
public class CustomLightCellsDataProvider : LightCellsDataProvider
{
private List<string> items = new List<string> { "Apple", "Banana", "Cherry", "Date", "Elderberry" };
private List<double> values = new List<double> { 1.99, 0.99, 2.99, 3.49, 4.99 };
private int currentRow = -1;
public bool StartSheet(int sheetIndex)
{
// Only process first sheet
return sheetIndex == 0;
}
public int NextRow()
{
currentRow++;
return currentRow < items.Count ? currentRow : -1;
}
public void StartRow(Row row)
{
// Set row height if needed
row.Height = 15;
}
public int NextCell()
{
if (currentRow == -1)
{
// Header row
return currentRow < 2 ? currentRow + 1 : -1;
}
else
{
return currentRow < 2 ? currentRow + 1 : -1;
}
}
public void StartCell(Cell cell)
{
if (currentRow == -1)
{
// Header
if (cell.Column == 0)
cell.Value = "Product";
else if (cell.Column == 1)
cell.Value = "Price";
}
else
{
// Data
if (cell.Column == 0)
cell.Value = items[currentRow];
else if (cell.Column == 1)
cell.Value = values[currentRow];
}
}
public bool IsGatherString()
{
return false;
}
}
}
```
### See Also
* interface [LightCellsDataProvider](../../lightcellsdataprovider/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
