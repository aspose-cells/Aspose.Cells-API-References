##Worksheet.IsSelected
Worksheet property. Indicates whether this worksheet is selected when the workbook is opened
## Worksheet.IsSelected property
Indicates whether this worksheet is selected when the workbook is opened.
```csharp
public bool IsSelected { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyIsSelectedDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a second worksheet
workbook.Worksheets.Add("Sheet2");
// Get the first worksheet
Worksheet worksheet1 = workbook.Worksheets[0];
worksheet1.Name = "FirstSheet";
// Get the second worksheet
Worksheet worksheet2 = workbook.Worksheets[1];
worksheet2.Name = "SecondSheet";
// Demonstrate IsSelected property
Console.WriteLine("Before selection:");
Console.WriteLine($"Worksheet1 IsSelected: {worksheet1.IsSelected}");
Console.WriteLine($"Worksheet2 IsSelected: {worksheet2.IsSelected}");
// Select the second worksheet
worksheet2.IsSelected = true;
workbook.Worksheets.ActiveSheetIndex = worksheet2.Index;
Console.WriteLine("\nAfter selection:");
Console.WriteLine($"Worksheet1 IsSelected: {worksheet1.IsSelected}");
Console.WriteLine($"Worksheet2 IsSelected: {worksheet2.IsSelected}");
// Save the workbook
workbook.Save("WorksheetSelectionDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
