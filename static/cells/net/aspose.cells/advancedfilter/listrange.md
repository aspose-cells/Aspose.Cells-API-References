##AdvancedFilter.ListRange
AdvancedFilter property. Gets the list range of this advanced filter
## AdvancedFilter.ListRange property
Gets the list range of this advanced filter.
```csharp
public string ListRange { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class AdvancedFilterPropertyListRangeDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Populate sample data
sheet.Cells["A1"].PutValue("Name");
sheet.Cells["B1"].PutValue("Age");
for (int i = 2; i <= 10; i++)
{
sheet.Cells["A" + i].PutValue("Person " + (i-1));
sheet.Cells["B" + i].PutValue(20 + i);
}
// Set up advanced filter
AdvancedFilter filter = sheet.GetAdvancedFilter();
// ListRange is read-only and set automatically when creating the filter
// We can only read it, not set it directly
// Display the list range (will show the automatically determined range)
Console.WriteLine("Advanced Filter List Range: " + filter.ListRange);
// Save the workbook
workbook.Save("AdvancedFilterDemo.xlsx");
}
}
}
```
### See Also
* class [AdvancedFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
