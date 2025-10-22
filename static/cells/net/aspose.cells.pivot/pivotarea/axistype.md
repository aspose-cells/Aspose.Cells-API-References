##PivotArea.AxisType
PivotArea property. Gets and sets the region of the PivotTable to which this rule applies
## PivotArea.AxisType property
Gets and sets the region of the PivotTable to which this rule applies.
```csharp
public PivotFieldType AxisType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotAreaPropertyAxisTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].Value = "Category";
worksheet.Cells["A2"].Value = "Electronics";
worksheet.Cells["A3"].Value = "Clothing";
worksheet.Cells["B1"].Value = "Sales";
worksheet.Cells["B2"].Value = 1000;
worksheet.Cells["B3"].Value = 800;
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add fields to pivot areas
pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);  // Sales
// Create and configure PivotArea
PivotArea pivotArea = new PivotArea(pivotTable);
pivotArea.AxisType = PivotFieldType.Row; // Demonstrate AxisType property
pivotArea.RuleType = PivotAreaType.Normal;
// Select the pivot area
pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.LabelOnly);
// Save the workbook
workbook.Save("PivotAreaAxisTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
