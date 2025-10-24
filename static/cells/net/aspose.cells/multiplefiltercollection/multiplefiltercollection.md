##MultipleFilterCollection.MultipleFilterCollection
MultipleFilterCollection constructor. Constructs one new instance
## MultipleFilterCollection constructor
Constructs one new instance.
```csharp
public MultipleFilterCollection()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class MultipleFilterCollectionMethodCtorDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
Cells cells = sheet.Cells;
// Populate sample data
cells[0, 0].PutValue("Data");
cells[1, 0].PutValue("abc");
cells[2, 0].PutValue("def");
cells[3, 0].PutValue("ghi");
cells[4, 0].PutValue("abc");
cells[5, 0].PutValue("jkl");
// Create auto filter and set filter type
sheet.AutoFilter.Range = "A1:A6";
FilterColumn fc = sheet.AutoFilter.FilterColumns[0];
fc.FilterType = FilterType.MultipleFilters;
// Create MultipleFilterCollection using constructor
MultipleFilterCollection mfc = new MultipleFilterCollection();
mfc.Add("abc");
mfc.Add("ghi");
fc.Filter = mfc;
// Apply filter
sheet.AutoFilter.Refresh();
// Output filtered results
Console.WriteLine("Filtered Rows:");
for (int row = 1; row <= 5; row++)
{
if (!cells.IsRowHidden(row))
{
Console.WriteLine(cells[row, 0].StringValue);
}
}
}
}
}
```
### See Also
* class [MultipleFilterCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
