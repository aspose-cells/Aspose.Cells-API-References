##Worksheet.HasAutofilter
Worksheet property. Indicates whether this worksheet has auto filter
## Worksheet.HasAutofilter property
Indicates whether this worksheet has auto filter.
```csharp
public bool HasAutofilter { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyHasAutofilterDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["A3"].PutValue("Alice");
worksheet.Cells["B3"].PutValue(25);
// Set autofilter
worksheet.AutoFilter.Range = "A1:B3";
// Check if worksheet has autofilter
Console.WriteLine("Worksheet has autofilter: " + worksheet.HasAutofilter);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
