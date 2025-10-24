##PivotField.DataDisplayFormat
PivotField property. Represents how to display the values in a data field of the pivot report
## PivotField.DataDisplayFormat property
Represents how to display the values in a data field of the pivot report.
```csharp
[Obsolete("Use PivotField.ShowValuesSetting.CalculationType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotFieldDataDisplayFormat DataDisplayFormat { get; set; }
```
### Remarks
NOTE: This property is now obsolete. Instead, please use PivotField.ShowValuesSetting.CalculationType property instead. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldPropertyDataDisplayFormatDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
Cells cells = sheet.Cells;
// Add sample data
cells["A1"].Value = "Product";
cells["B1"].Value = "Quarter";
cells["C1"].Value = "Sales";
cells["A2"].Value = "Laptop";
cells["A3"].Value = "Phone";
cells["A4"].Value = "Tablet";
cells["A5"].Value = "Laptop";
cells["A6"].Value = "Phone";
cells["A7"].Value = "Tablet";
cells["B2"].Value = "Q1";
cells["B3"].Value = "Q1";
cells["B4"].Value = "Q1";
cells["B5"].Value = "Q2";
cells["B6"].Value = "Q2";
cells["B7"].Value = "Q2";
cells["C2"].Value = 1000;
cells["C3"].Value = 1500;
cells["C4"].Value = 800;
cells["C5"].Value = 1200;
cells["C6"].Value = 1800;
cells["C7"].Value = 900;
// Create pivot table
int pivotIndex = sheet.PivotTables.Add("A1:C7", "E3", "SalesPivot");
PivotTable pivot = sheet.PivotTables[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "Product");
pivot.AddFieldToArea(PivotFieldType.Column, "Quarter");
int fieldIndex = pivot.AddFieldToArea(PivotFieldType.Data, "Sales");
PivotField dataField = pivot.DataFields[fieldIndex];
// Set display format to show values as percentage of total
dataField.DataDisplayFormat = PivotFieldDataDisplayFormat.PercentageOfTotal;
dataField.DisplayName = "Sales % of Total";
pivot.RefreshData();
pivot.CalculateData();
workbook.Save("PivotFieldDataDisplayFormatDemo.xlsx");
}
}
}
```
### See Also
* enum [PivotFieldDataDisplayFormat](../../pivotfielddatadisplayformat/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
