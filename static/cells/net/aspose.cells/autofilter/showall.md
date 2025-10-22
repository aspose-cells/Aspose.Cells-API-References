##AutoFilter.ShowAll
AutoFilter method. Unhide all rows
## AutoFilter.ShowAll method
Unhide all rows.
```csharp
public void ShowAll()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class AutoFilterMethodShowAllDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Fruit");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Banana");
worksheet.Cells["A4"].PutValue("Orange");
worksheet.Cells["A5"].PutValue("Grape");
// Apply auto filter
worksheet.AutoFilter.Range = "A1:A5";
// Filter to show only "Apple"
worksheet.AutoFilter.Filter(0, "Apple");
// Show all data again
worksheet.AutoFilter.ShowAll();
// Save the workbook
workbook.Save("ShowAllDemoOutput.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
