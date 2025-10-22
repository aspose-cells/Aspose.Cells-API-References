##Enum PivotTableAutoFormatType
Aspose.Cells.Pivot.PivotTableAutoFormatType enum. Represents PivotTable auto format type
## PivotTableAutoFormatType enumeration
Represents PivotTable auto format type.
```csharp
public enum PivotTableAutoFormatType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | `0` | Represents None format type. |
| Classic | `1` | Represents Classic auto format type. |
| Report1 | `2` | Represents Report1 format type. |
| Report2 | `3` | Represents Report2 format type. |
| Report3 | `4` | Represents Report3 format type. |
| Report4 | `5` | Represents Report4 format type. |
| Report5 | `6` | Represents Report5 format type. |
| Report6 | `7` | Represents Report6 format type. |
| Report7 | `8` | Represents Report7 format type. |
| Report8 | `9` | Represents Report8 format type. |
| Report9 | `10` | Represents Report9 format type. |
| Report10 | `11` | Represents Report10 format type. |
| Table1 | `12` | Represents Table1 format type. |
| Table2 | `13` | Represents Table2 format type. |
| Table3 | `14` | Represents Table3 format type. |
| Table4 | `15` | Represents Table4 format type. |
| Table5 | `16` | Represents Table5 format type. |
| Table6 | `17` | Represents Table6 format type. |
| Table7 | `18` | Represents Table7 format type. |
| Table8 | `19` | Represents Table8 format type. |
| Table9 | `20` | Represents Table9 format type. |
| Table10 | `21` | Represents Table10 format type. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotTableAutoFormatTypeDemo
{
public static void PivotTableAutoFormatTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data for the PivotTable
worksheet.Cells[0, 0].Value = "Fruit";
worksheet.Cells[0, 1].Value = "Year";
worksheet.Cells[0, 2].Value = "Amount";
worksheet.Cells[1, 0].Value = "Apple";
worksheet.Cells[1, 1].Value = 2020;
worksheet.Cells[1, 2].Value = 50;
worksheet.Cells[2, 0].Value = "Banana";
worksheet.Cells[2, 1].Value = 2020;
worksheet.Cells[2, 2].Value = 60;
worksheet.Cells[3, 0].Value = "Apple";
worksheet.Cells[3, 1].Value = 2021;
worksheet.Cells[3, 2].Value = 70;
worksheet.Cells[4, 0].Value = "Banana";
worksheet.Cells[4, 1].Value = 2021;
worksheet.Cells[4, 2].Value = 80;
// Add a PivotTable to the worksheet
int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:C5", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add fields to the PivotTable
pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount
// Set the auto format type for the PivotTable
pivotTable.AutoFormatType = PivotTableAutoFormatType.Report1;
// Save the workbook
workbook.Save("PivotTableAutoFormatTypeExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)
