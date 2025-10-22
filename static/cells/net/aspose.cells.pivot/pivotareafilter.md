##Class PivotAreaFilter
Aspose.Cells.Pivot.PivotAreaFilter class. Represents the filter of PivotArea for PivotTable
## PivotAreaFilter class
Represents the filter of [`PivotArea`](../pivotarea/) for [`PivotTable`](../pivottable/).
```csharp
public class PivotAreaFilter
```
## Constructors
| Name | Description |
| --- | --- |
| [PivotAreaFilter](pivotareafilter/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [Selected](../../aspose.cells.pivot/pivotareafilter/selected/) { get; set; } | Indicates whether this field has selection. Only works when the PivotTable is in Outline view. |
## Methods
| Name | Description |
| --- | --- |
| [IsSubtotalSet](../../aspose.cells.pivot/pivotareafilter/issubtotalset/)(PivotFieldSubtotalType) | Gets which subtotal is set for this filter. |
| [SetSubtotals](../../aspose.cells.pivot/pivotareafilter/setsubtotals/)(PivotFieldSubtotalType, bool) | Subtotal for the filter. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotClassPivotAreaFilterDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Sample data setup
worksheet.Cells["A1"].Value = "Product";
worksheet.Cells["A2"].Value = "Bike";
worksheet.Cells["A3"].Value = "Car";
worksheet.Cells["B1"].Value = "Sales";
worksheet.Cells["B2"].Value = 1000;
worksheet.Cells["B3"].Value = 2000;
// Create PivotTable - fix return value handling
int pivotIndex = worksheet.PivotTables.Add("A1:B3", "E5", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Create and configure PivotAreaFilter
PivotAreaFilter filter = new PivotAreaFilter();
filter.Selected = true;
filter.SetSubtotals(PivotFieldSubtotalType.Sum, true);
// Demonstrate methods
bool isSumSet = filter.IsSubtotalSet(PivotFieldSubtotalType.Sum);
Console.WriteLine($"Sum subtotal visibility set: {isSumSet}");
workbook.Save("PivotAreaFilterDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)
