##AutoFilter.Range
AutoFilter property. Represents the range to which the specified AutoFilter applies
## AutoFilter.Range property
Represents the range to which the specified AutoFilter applies.
```csharp
public string Range { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class AutoFilterPropertyRangeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue("Header");
sheet.Cells["A2"].PutValue("Item1");
sheet.Cells["A3"].PutValue("Item2");
sheet.Cells["A4"].PutValue("Item3");
sheet.Cells["A5"].PutValue("Item4");
// Apply auto filter to range A1:A5
sheet.AutoFilter.Range = "A1:A5";
// Display the auto filter range
Console.WriteLine("AutoFilter Range: " + sheet.AutoFilter.Range);
// Save the workbook
workbook.Save("AutoFilterRangeDemo.xlsx");
}
}
}
```
### See Also
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
