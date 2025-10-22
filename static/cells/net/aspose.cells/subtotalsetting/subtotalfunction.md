##SubtotalSetting.SubtotalFunction
SubtotalSetting property. The subtotal function
## SubtotalSetting.SubtotalFunction property
The subtotal function.
```csharp
public ConsolidationFunction SubtotalFunction { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class SubtotalSettingPropertySubtotalFunctionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Value");
for (int i = 2; i <= 10; i++)
{
worksheet.Cells["A" + i].PutValue(i % 2 == 0 ? "Group A" : "Group B");
worksheet.Cells["B" + i].PutValue(i * 100);
}
// Create subtotal setting by retrieving from existing data
CellArea area = CellArea.CreateCellArea("A1", "B10");
SubtotalSetting subtotalSetting = worksheet.Cells.RetrieveSubtotalSetting(area);
// Configure subtotal - these properties are read-only in the actual API
// So we'll use the Subtotal method directly with parameters
int groupBy = 0; // Group by first column
ConsolidationFunction function = ConsolidationFunction.Sum;
int[] subtotalColumns = new int[] {1}; // Subtotal on second column
// Apply subtotals
worksheet.Cells.Subtotal(area, groupBy, function, subtotalColumns);
// Verify the SubtotalFunction property from the retrieved setting
Console.WriteLine("Subtotal Function: " + subtotalSetting.SubtotalFunction);
// Save the workbook
workbook.Save("SubtotalDemo.xlsx");
}
}
}
```
### See Also
* enum [ConsolidationFunction](../../consolidationfunction/)
* class [SubtotalSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
