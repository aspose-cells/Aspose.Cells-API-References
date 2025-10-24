##PivotField.BaseFieldIndex
PivotField property. Represents the base field for a custom calculation when the ShowDataAs calculation is in use
## PivotField.BaseFieldIndex property
Represents the base field for a custom calculation when the ShowDataAs calculation is in use.
```csharp
[Obsolete("Use PivotField.ShowValuesSetting.BaseFieldIndex property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int BaseFieldIndex { get; set; }
```
### Remarks
NOTE: This property is now obsolete. Instead, please use PivotField.ShowValuesSetting.BaseFieldIndex property instead. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldPropertyBaseFieldIndexDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Add sample data
cells["A1"].Value = "Category";
cells["B1"].Value = "Quarter";
cells["C1"].Value = "Sales";
cells["A2"].Value = "Electronics";
cells["A3"].Value = "Electronics";
cells["A4"].Value = "Clothing";
cells["A5"].Value = "Clothing";
cells["B2"].Value = "Q1";
cells["B3"].Value = "Q2";
cells["B4"].Value = "Q1";
cells["B5"].Value = "Q2";
cells["C2"].Value = 1000;
cells["C3"].Value = 1500;
cells["C4"].Value = 800;
cells["C5"].Value = 1200;
// Create pivot table - get index first then get the table
int pivotIndex = worksheet.PivotTables.Add("A1:C5", "E3", "SalesPivotTable");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add fields to pivot areas
pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
pivotTable.AddFieldToArea(PivotFieldType.Column, "Quarter");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Get the row field and set BaseFieldIndex
PivotField rowField = pivotTable.RowFields[0];
rowField.BaseFieldIndex = 0; // Base field is itself (Category)
rowField.BaseItemPosition = PivotItemPosition.Previous; // Compare to previous item
// Refresh pivot table
pivotTable.RefreshData();
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotFieldBaseFieldIndexDemo.xlsx");
}
}
}
```
### See Also
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
