##CustomFilter.Criteria
CustomFilter property. Gets and sets the criteria
## CustomFilter.Criteria property
Gets and sets the criteria.
```csharp
public object Criteria { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CustomFilterPropertyCriteriaDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Numbers");
worksheet.Cells["A2"].PutValue(2);
worksheet.Cells["A3"].PutValue(7);
worksheet.Cells["A4"].PutValue(5);
worksheet.Cells["A5"].PutValue(9);
worksheet.Cells["A6"].PutValue(3);
// Apply auto filter
worksheet.AutoFilter.Range = "A1:A6";
AutoFilter autoFilter = worksheet.AutoFilter;
// Add custom filter
int fieldIndex = 0;
autoFilter.Custom(fieldIndex, FilterOperatorType.GreaterOrEqual, 5);
// Get the filter column and display criteria
FilterColumn fc = autoFilter.FilterColumns[fieldIndex];
CustomFilter cf = ((CustomFilterCollection)fc.Filter)[0];
Console.WriteLine("Filter Criteria: " + cf.Criteria);
// Refresh the filter
autoFilter.Refresh();
// Save the workbook
workbook.Save("CustomFilterExample.xlsx");
}
}
}
```
### See Also
* class [CustomFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
