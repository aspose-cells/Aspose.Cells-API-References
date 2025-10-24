##Cells.RetrieveSubtotalSetting
Cells method. Retrieves subtotals setting of the range
## Cells.RetrieveSubtotalSetting method
Retrieves subtotals setting of the range.
```csharp
public SubtotalSetting RetrieveSubtotalSetting(CellArea ca)
```
| Parameter | Type | Description |
| --- | --- | --- |
| ca | CellArea | The range |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodRetrieveSubtotalSettingWithCellAreaDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for subtotals
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Value");
for (int i = 2; i <= 10; i++)
{
worksheet.Cells["A" + i].PutValue(i % 2 == 0 ? "Group1" : "Group2");
worksheet.Cells["B" + i].PutValue(i * 100);
}
// Create subtotals
CellArea area = CellArea.CreateCellArea("A1", "B10");
worksheet.Cells.Subtotal(area, 0, ConsolidationFunction.Sum, new int[] { 1 });
// Retrieve subtotal settings
SubtotalSetting setting = worksheet.Cells.RetrieveSubtotalSetting(area);
// Output settings
Console.WriteLine("GroupBy: " + setting.GroupBy);
Console.WriteLine("Function: " + setting.SubtotalFunction);
Console.WriteLine("SummaryBelowData: " + setting.SummaryBelowData);
Console.WriteLine("TotalList: " + string.Join(",", setting.TotalList));
}
}
}
```
### See Also
* class [SubtotalSetting](../../subtotalsetting/)
* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
