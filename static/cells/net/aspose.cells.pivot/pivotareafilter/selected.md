##PivotAreaFilter.Selected
PivotAreaFilter property. Indicates whether this field has selection. Only works when the PivotTable is in Outline view
## PivotAreaFilter.Selected property
Indicates whether this field has selection. Only works when the PivotTable is in Outline view.
```csharp
public bool Selected { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotAreaFilterPropertySelectedDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].Value = "Fruit";
worksheet.Cells["A2"].Value = "Apple";
worksheet.Cells["A3"].Value = "Orange";
worksheet.Cells["A4"].Value = "Banana";
worksheet.Cells["B1"].Value = "Sales";
worksheet.Cells["B2"].Value = 1000;
worksheet.Cells["B3"].Value = 2000;
worksheet.Cells["B4"].Value = 3000;
// Create a pivot table
int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Get pivot area filter
PivotArea pivotArea = new PivotArea(pivotTable);
PivotAreaFilter filter = pivotArea.Filters[0];
// Display current Selected value
Console.WriteLine("Current Selected value: " + filter.Selected);
// Change Selected value (only affects Outline view)
filter.Selected = true;
Console.WriteLine("New Selected value: " + filter.Selected);
// Save the workbook
workbook.Save("PivotAreaFilterSelectedDemo.xlsx");
}
}
}
```
### See Also
* class [PivotAreaFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
