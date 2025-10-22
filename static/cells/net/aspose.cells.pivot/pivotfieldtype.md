##Enum PivotFieldType
Aspose.Cells.Pivot.PivotFieldType enum. Represents PivotTable field type
## PivotFieldType enumeration
Represents PivotTable field type.
```csharp
public enum PivotFieldType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Undefined | `0` | Presents base pivot field type. |
| Row | `1` | Presents row pivot field type. |
| Column | `2` | Presents column pivot field type. |
| Page | `4` | Presents page pivot field type. |
| Data | `8` | Presents data pivot field type. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotFieldTypeDemo
{
public static void PivotFieldTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data
worksheet.Cells[0, 0].Value = "Fruit";
worksheet.Cells[1, 0].Value = "Grape";
worksheet.Cells[2, 0].Value = "Blueberry";
worksheet.Cells[3, 0].Value = "Kiwi";
worksheet.Cells[4, 0].Value = "Cherry";
worksheet.Cells[5, 0].Value = "Grape";
worksheet.Cells[6, 0].Value = "Blueberry";
worksheet.Cells[7, 0].Value = "Kiwi";
worksheet.Cells[8, 0].Value = "Cherry";
worksheet.Cells[0, 1].Value = "Year";
worksheet.Cells[1, 1].Value = 2020;
worksheet.Cells[2, 1].Value = 2020;
worksheet.Cells[3, 1].Value = 2020;
worksheet.Cells[4, 1].Value = 2020;
worksheet.Cells[5, 1].Value = 2021;
worksheet.Cells[6, 1].Value = 2021;
worksheet.Cells[7, 1].Value = 2021;
worksheet.Cells[8, 1].Value = 2021;
worksheet.Cells[0, 2].Value = "Amount";
worksheet.Cells[1, 2].Value = 50;
worksheet.Cells[2, 2].Value = 60;
worksheet.Cells[3, 2].Value = 70;
worksheet.Cells[4, 2].Value = 80;
worksheet.Cells[5, 2].Value = 90;
worksheet.Cells[6, 2].Value = 100;
worksheet.Cells[7, 2].Value = 110;
worksheet.Cells[8, 2].Value = 120;
// Add a pivot table
PivotTableCollection pivotTables = worksheet.PivotTables;
int pivotIndex = pivotTables.Add("=Sheet1!A1:C9", "A12", "PivotTable1");
PivotTable pivotTable = pivotTables[pivotIndex];
// Add fields to the pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount
// Set pivot table style
pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium9;
// Refresh and calculate data
pivotTable.RefreshData();
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotFieldTypeExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)
