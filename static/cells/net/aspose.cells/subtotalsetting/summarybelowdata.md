##SubtotalSetting.SummaryBelowData
SubtotalSetting property. Indicates whether add summary below data
## SubtotalSetting.SummaryBelowData property
Indicates whether add summary below data.
```csharp
public bool SummaryBelowData { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class SubtotalSettingPropertySummaryBelowDataDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("A");
worksheet.Cells["A4"].PutValue("B");
worksheet.Cells["A5"].PutValue("B");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
worksheet.Cells["B5"].PutValue(40);
// Create cell area for subtotals
CellArea area = CellArea.CreateCellArea("A1", "B5");
// Apply subtotals using Cells.Subtotal method with all required parameters
worksheet.Cells.Subtotal(
area,
0,
ConsolidationFunction.Sum,
new int[] { 1 },
false,
false,
false);  // summaryBelowData parameter
// Retrieve the setting to check SummaryBelowData
SubtotalSetting retrievedSetting = worksheet.Cells.RetrieveSubtotalSetting(area);
// Output the SummaryBelowData property value
Console.WriteLine("SummaryBelowData: " + retrievedSetting.SummaryBelowData);
}
}
}
```
### See Also
* class [SubtotalSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
