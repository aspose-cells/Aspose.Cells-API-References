##AutoFilter.Filter
AutoFilter method. Filters a list with specified criteria
## AutoFilter.Filter method
Filters a list with specified criteria.
```csharp
public void Filter(int fieldIndex, string criteria)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| criteria | String | The specified criteria (a string; for example, "101"). |
### Remarks
Aspose.Cells will remove all other filter setting on this field as Ms Excel 97-2003.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class AutoFilterMethodFilterWithInt32StringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue("Name");
sheet.Cells["A2"].PutValue("Nom1");
sheet.Cells["A3"].PutValue("Nom2");
sheet.Cells["A4"].PutValue("Nom3");
sheet.Cells["A5"].PutValue("Nom2");
// Apply auto filter using correct SetRange parameters
sheet.AutoFilter.SetRange(0, 0, 4); // startRow: 0, startColumn: 0, endRow: 4
sheet.AutoFilter.Filter(0, "Nom2"); // Filter column 0 (A) for "Nom2"
sheet.AutoFilter.Refresh();
// Save the result
workbook.Save("AutoFilterDemo.xlsx");
}
}
}
```
### See Also
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
