##Enum PivotFieldDataDisplayFormat
Aspose.Cells.Pivot.PivotFieldDataDisplayFormat enum. Represents data display format in the PivotTable data field
## PivotFieldDataDisplayFormat enumeration
Represents data display format in the PivotTable data field.
```csharp
public enum PivotFieldDataDisplayFormat
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Normal | `0` | Represents normal display format. |
| DifferenceFrom | `1` | Represents difference from display format. |
| PercentageOf | `2` | Represents percentage of display format. |
| PercentageDifferenceFrom | `3` | Represents percentage difference from display format. |
| RunningTotalIn | `4` | Represents running total in display format. |
| PercentageOfRow | `5` | Represents percentage of row display format. |
| PercentageOfColumn | `6` | Represents percentage of column display format. |
| PercentageOfTotal | `7` | Represents percentage of total display format. |
| Index | `8` | Represents index display format. |
| PercentageOfParentRowTotal | `9` | Represents percentage of parent row total display format. |
| PercentageOfParentColumnTotal | `10` | Represents percentage of parent column total display format. |
| PercentageOfParentTotal | `11` | Represents percentage of parent total display format. |
| PercentageOfRunningTotalIn | `12` | Represents percentage of running total in display format. |
| RankSmallestToLargest | `13` | Represents smallest to largest display format. |
| RankLargestToSmallest | `14` | Represents largest to smallest display format. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotFieldDataDisplayFormatDemo
{
public static void PivotFieldDataDisplayFormatExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
Cells cells = sheet.Cells;
// Add some sample data
cells[0, 0].Value = "fruit";
cells[1, 0].Value = "grape";
cells[2, 0].Value = "blueberry";
cells[3, 0].Value = "kiwi";
cells[4, 0].Value = "cherry";
cells[5, 0].Value = "grape";
cells[6, 0].Value = "blueberry";
cells[7, 0].Value = "kiwi";
cells[8, 0].Value = "cherry";
cells[0, 1].Value = "year";
cells[1, 1].Value = 2020;
cells[2, 1].Value = 2020;
cells[3, 1].Value = 2020;
cells[4, 1].Value = 2020;
cells[5, 1].Value = 2021;
cells[6, 1].Value = 2021;
cells[7, 1].Value = 2021;
cells[8, 1].Value = 2021;
cells[0, 2].Value = "amount";
cells[1, 2].Value = 50;
cells[2, 2].Value = 60;
cells[3, 2].Value = 70;
cells[4, 2].Value = 80;
cells[5, 2].Value = 90;
cells[6, 2].Value = 100;
cells[7, 2].Value = 110;
cells[8, 2].Value = 120;
// Add a pivot table
PivotTableCollection pivots = sheet.PivotTables;
int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
PivotTable pivot = pivots[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "year");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");
// Set the pivot table style
pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
// Change PivotField's attributes
PivotField dataField = pivot.DataFields[0];
dataField.DisplayName = "custom display name";
// Set DataDisplayFormat
dataField.DataDisplayFormat = PivotFieldDataDisplayFormat.PercentageOfTotal;
// Refresh and calculate data
pivot.RefreshData();
pivot.CalculateData();
// Save the workbook
workbook.Save("PivotFieldDataDisplayFormatExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)
