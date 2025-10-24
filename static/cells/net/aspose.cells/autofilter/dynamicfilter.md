##AutoFilter.DynamicFilter
AutoFilter method. Adds a dynamic filter
## AutoFilter.DynamicFilter method
Adds a dynamic filter.
```csharp
public void DynamicFilter(int fieldIndex, DynamicFilterType dynamicFilterType)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| dynamicFilterType | DynamicFilterType | Dynamic filter type. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class AutoFilterMethodDynamicFilterWithInt32DynamicFilterTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Date");
worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
worksheet.Cells["A5"].PutValue(new DateTime(2023, 4, 1));
worksheet.Cells["A6"].PutValue(new DateTime(2023, 5, 1));
// Apply auto filter using the correct method signature
worksheet.AutoFilter.Range = "A1:A6";
// Apply dynamic filter for March dates
worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.March);
workbook.Save("DynamicFilterDemo.xlsx");
}
}
}
```
### See Also
* enum [DynamicFilterType](../../dynamicfiltertype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
