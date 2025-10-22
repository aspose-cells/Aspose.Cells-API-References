##PivotShowValuesSetting.CalculationType
PivotShowValuesSetting property. Represents how to show values of a data field in the pivot report
## PivotShowValuesSetting.CalculationType property
Represents how to show values of a data field in the pivot report.
```csharp
public PivotFieldDataDisplayFormat CalculationType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotShowValuesSettingPropertyCalculationTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for pivot table
Cells cells = sheet.Cells;
cells["A1"].Value = "Fruit";
cells["B1"].Value = "Quantity";
cells["A2"].Value = "Apple";
cells["B2"].Value = 10;
cells["A3"].Value = "Orange";
cells["B3"].Value = 20;
cells["A4"].Value = "Banana";
cells["B4"].Value = 15;
cells["A5"].Value = "Apple";
cells["B5"].Value = 5;
// Create pivot table
int index = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
// Add data field and set calculation type
pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
PivotField dataField = pivotTable.DataFields[0];
dataField.ShowValuesSetting.CalculationType = PivotFieldDataDisplayFormat.RankLargestToSmallest;
// Calculate data and save
pivotTable.CalculateData();
workbook.Save("PivotShowValuesSettingPropertyCalculationTypeDemo_out.xlsx");
}
}
}
```
### See Also
* enum [PivotFieldDataDisplayFormat](../../pivotfielddatadisplayformat/)
* class [PivotShowValuesSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
