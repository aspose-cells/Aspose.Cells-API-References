##MultipleFilterCollection.Add
MultipleFilterCollection method. Adds string filter
## MultipleFilterCollection.Add method
Adds string filter.
```csharp
public void Add(string filter)
```
| Parameter | Type | Description |
| --- | --- | --- |
| filter | String | The filter data. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class MultipleFilterCollectionMethodAddWithStringDemo
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
// Apply filter
sheet.AutoFilter.Range = "A1:A5";
FilterColumn fc = sheet.AutoFilter.FilterColumns[0];
fc.FilterType = FilterType.MultipleFilters;
MultipleFilterCollection mfc = new MultipleFilterCollection();
mfc.Add("abc");  // Demonstrate Add method with string parameter
mfc.Add("ghi");
fc.Filter = mfc;
sheet.AutoFilter.Refresh();
// Output filtered results
Console.WriteLine("Filtered Rows:");
for (int i = 1; i <= 4; i++)
{
if (!cells.IsRowHidden(i))
{
Console.WriteLine(cells[i, 0].StringValue);
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
