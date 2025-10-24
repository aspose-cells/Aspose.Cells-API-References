##Enum PivotMissingItemLimitType
Aspose.Cells.Pivot.PivotMissingItemLimitType enum. Represents number of items to retain per field
## PivotMissingItemLimitType enumeration
Represents number of items to retain per field.
```csharp
public enum PivotMissingItemLimitType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Automatic | `0` | The default number of unique items per PivotField allowed. |
| Max | `1` | The maximum number of unique items per PivotField allowed (&gt;32,500). |
| None | `2` | No unique items per PivotField allowed. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotMissingItemLimitTypeDemo
{
public static void PivotMissingItemLimitTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Add some sample data
cells[0, 0].Value = "Fruit";
cells[0, 1].Value = "Year";
cells[0, 2].Value = "Amount";
cells[1, 0].Value = "Apple";
cells[1, 1].Value = 2020;
cells[1, 2].Value = 50;
cells[2, 0].Value = "Banana";
cells[2, 1].Value = 2020;
cells[2, 2].Value = 60;
cells[3, 0].Value = "Apple";
cells[3, 1].Value = 2021;
cells[3, 2].Value = 70;
cells[4, 0].Value = "Banana";
cells[4, 1].Value = 2021;
cells[4, 2].Value = 80;
// Add a pivot table to the worksheet
PivotTableCollection pivotTables = worksheet.PivotTables;
int index = pivotTables.Add("=Sheet1!A1:C5", "E3", "PivotTable1");
PivotTable pivotTable = pivotTables[index];
// Add fields to the pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount
// Set the MissingItemsLimit property
pivotTable.MissingItemsLimit = PivotMissingItemLimitType.Max;
// Refresh and calculate the pivot table data
pivotTable.RefreshData();
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotMissingItemLimitTypeExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)
