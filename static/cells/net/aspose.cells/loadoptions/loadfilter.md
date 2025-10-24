##LoadOptions.LoadFilter
LoadOptions property. The filter to denote how to load data
## LoadOptions.LoadFilter property
The filter to denote how to load data.
```csharp
public LoadFilter LoadFilter { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CustomLoadFilter : LoadFilter
{
public override void StartSheet(Worksheet sheet)
{
// Only load data if sheet is visible
if (sheet.IsVisible)
{
base.StartSheet(sheet);
}
}
}
public class LoadOptionsPropertyLoadFilterDemo
{
public static void Run()
{
// Create a test workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
sheet.Name = "HiddenSheet";
sheet.IsVisible = false;
sheet.Cells["A1"].PutValue("This should not load");
// Add a visible sheet
Worksheet visibleSheet = workbook.Worksheets.Add("VisibleSheet");
visibleSheet.Cells["A1"].PutValue("This will load");
// Save the test file
string filePath = "LoadFilterTest.xlsx";
workbook.Save(filePath);
workbook.Dispose();
// Load with custom filter
LoadOptions options = new LoadOptions();
options.LoadFilter = new CustomLoadFilter();
Workbook loadedWorkbook = new Workbook(filePath, options);
// Verify only visible sheet loaded
Console.WriteLine("Loaded Sheets:");
foreach (Worksheet ws in loadedWorkbook.Worksheets)
{
Console.WriteLine($"- {ws.Name}: Visible={ws.IsVisible}");
if (ws.IsVisible)
{
Console.WriteLine($"  A1 Value: {ws.Cells["A1"].StringValue}");
}
}
loadedWorkbook.Dispose();
}
}
}
```
### See Also
* class [LoadFilter](../../loadfilter/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
