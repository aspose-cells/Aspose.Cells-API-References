##AutoFilter.FilterColumns
AutoFilter property. Gets the collection of the filter columns
## AutoFilter.FilterColumns property
Gets the collection of the filter columns.
```csharp
public FilterColumnCollection FilterColumns { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class AutoFilterPropertyFilterColumnsDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Department");
worksheet.Cells["B1"].PutValue("Name");
worksheet.Cells["C1"].PutValue("Status");
worksheet.Cells["A2"].PutValue("HR");
worksheet.Cells["B2"].PutValue("John");
worksheet.Cells["C2"].PutValue("Present");
worksheet.Cells["A3"].PutValue("IT");
worksheet.Cells["B3"].PutValue("Sarah");
worksheet.Cells["C3"].PutValue("Absent");
worksheet.Cells["A4"].PutValue("HR");
worksheet.Cells["B4"].PutValue("Mike");
worksheet.Cells["C4"].PutValue("Present");
// Apply auto filter
AutoFilter autoFilter = worksheet.AutoFilter;
autoFilter.Range = "A1:C1";
// Filter column 2 (Status) for "Present" values
autoFilter.Filter(2, "Present");
// Access the filter column
FilterColumn filterColumn = autoFilter.FilterColumns[2];
// Save the workbook
workbook.Save("AutoFilterExample.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [FilterColumnCollection](../../filtercolumncollection/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
