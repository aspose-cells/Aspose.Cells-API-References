##FilterColumnCollection.GetByIndex
FilterColumnCollection method. Returns a single Filter object from a collection
## FilterColumnCollection.GetByIndex method
Returns a single Filter object from a collection.
```csharp
public FilterColumn GetByIndex(int index)
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FilterColumnCollectionMethodGetByIndexWithInt32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(25);
worksheet.Cells["A3"].PutValue("Jane");
worksheet.Cells["B3"].PutValue(30);
worksheet.AutoFilter.Range = "A1:B3";
FilterColumnCollection filterColumns = worksheet.AutoFilter.FilterColumns;
worksheet.AutoFilter.AddFilter(1, "25");
worksheet.AutoFilter.Refresh();
FilterColumn filterColumn = filterColumns.GetByIndex(0);
Console.WriteLine("Filter column index: " + filterColumn.FieldIndex);
workbook.Save("FilterColumnCollectionExample.xlsx");
}
}
}
```
### See Also
* class [FilterColumn](../../filtercolumn/)
* class [FilterColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
