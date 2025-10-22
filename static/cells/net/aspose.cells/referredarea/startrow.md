##ReferredArea.StartRow
ReferredArea property. The start row of the area
## ReferredArea.StartRow property
The start row of the area.
```csharp
public int StartRow { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ReferredAreaPropertyStartRowDemo
{
public static void Run()
{
// Create a workbook and worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Fill some sample data
worksheet.Cells["A1"].PutValue("Header");
worksheet.Cells["A2"].PutValue(10);
worksheet.Cells["A3"].PutValue(20);
worksheet.Cells["A4"].PutValue(30);
// Create a named range that refers to A2:A4
int index = workbook.Worksheets.Names.Add("MyRange");
Name name = workbook.Worksheets.Names[index];
name.RefersTo = "=Sheet1!$A$2:$A$4";
// Get the referred area with recalculate parameter
ReferredArea area = name.GetReferredAreas(false)[0];
// Demonstrate StartRow property
Console.WriteLine("Start Row: " + area.StartRow); // Should output 1 (0-based)
Console.WriteLine("End Row: " + area.EndRow);     // Should output 3 (0-based)
Console.WriteLine("Row Count: " + (area.EndRow - area.StartRow + 1)); // Should output 3
// Iterate through the referred area using StartRow and EndRow
for (int row = area.StartRow; row <= area.EndRow; row++)
{
Cell cell = worksheet.Cells[row, 0]; // Column 0 is A
Console.WriteLine("Value at row " + row + ": " + cell.Value);
}
}
}
}
```
### See Also
* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
