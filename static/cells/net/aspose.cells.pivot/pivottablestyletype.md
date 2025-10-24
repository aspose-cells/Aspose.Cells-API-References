##Enum PivotTableStyleType
Aspose.Cells.Pivot.PivotTableStyleType enum. Represents the pivot table style type
## PivotTableStyleType enumeration
Represents the pivot table style type.
```csharp
public enum PivotTableStyleType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | `0` |  |
| PivotTableStyleLight1 | `1` |  |
| PivotTableStyleLight2 | `2` |  |
| PivotTableStyleLight3 | `3` |  |
| PivotTableStyleLight4 | `4` |  |
| PivotTableStyleLight5 | `5` |  |
| PivotTableStyleLight6 | `6` |  |
| PivotTableStyleLight7 | `7` |  |
| PivotTableStyleLight8 | `8` |  |
| PivotTableStyleLight9 | `9` |  |
| PivotTableStyleLight10 | `10` |  |
| PivotTableStyleLight11 | `11` |  |
| PivotTableStyleLight12 | `12` |  |
| PivotTableStyleLight13 | `13` |  |
| PivotTableStyleLight14 | `14` |  |
| PivotTableStyleLight15 | `15` |  |
| PivotTableStyleLight16 | `16` |  |
| PivotTableStyleLight17 | `17` |  |
| PivotTableStyleLight18 | `18` |  |
| PivotTableStyleLight19 | `19` |  |
| PivotTableStyleLight20 | `20` |  |
| PivotTableStyleLight21 | `21` |  |
| PivotTableStyleLight22 | `22` |  |
| PivotTableStyleLight23 | `23` |  |
| PivotTableStyleLight24 | `24` |  |
| PivotTableStyleLight25 | `25` |  |
| PivotTableStyleLight26 | `26` |  |
| PivotTableStyleLight27 | `27` |  |
| PivotTableStyleLight28 | `28` |  |
| PivotTableStyleMedium1 | `29` |  |
| PivotTableStyleMedium2 | `30` |  |
| PivotTableStyleMedium3 | `31` |  |
| PivotTableStyleMedium4 | `32` |  |
| PivotTableStyleMedium5 | `33` |  |
| PivotTableStyleMedium6 | `34` |  |
| PivotTableStyleMedium7 | `35` |  |
| PivotTableStyleMedium8 | `36` |  |
| PivotTableStyleMedium9 | `37` |  |
| PivotTableStyleMedium10 | `38` |  |
| PivotTableStyleMedium11 | `39` |  |
| PivotTableStyleMedium12 | `40` |  |
| PivotTableStyleMedium13 | `41` |  |
| PivotTableStyleMedium14 | `42` |  |
| PivotTableStyleMedium15 | `43` |  |
| PivotTableStyleMedium16 | `44` |  |
| PivotTableStyleMedium17 | `45` |  |
| PivotTableStyleMedium18 | `46` |  |
| PivotTableStyleMedium19 | `47` |  |
| PivotTableStyleMedium20 | `48` |  |
| PivotTableStyleMedium21 | `49` |  |
| PivotTableStyleMedium22 | `50` |  |
| PivotTableStyleMedium23 | `51` |  |
| PivotTableStyleMedium24 | `52` |  |
| PivotTableStyleMedium25 | `53` |  |
| PivotTableStyleMedium26 | `54` |  |
| PivotTableStyleMedium27 | `55` |  |
| PivotTableStyleMedium28 | `56` |  |
| PivotTableStyleDark1 | `57` |  |
| PivotTableStyleDark2 | `58` |  |
| PivotTableStyleDark3 | `59` |  |
| PivotTableStyleDark4 | `60` |  |
| PivotTableStyleDark5 | `61` |  |
| PivotTableStyleDark6 | `62` |  |
| PivotTableStyleDark7 | `63` |  |
| PivotTableStyleDark8 | `64` |  |
| PivotTableStyleDark9 | `65` |  |
| PivotTableStyleDark10 | `66` |  |
| PivotTableStyleDark11 | `67` |  |
| PivotTableStyleDark12 | `68` |  |
| PivotTableStyleDark13 | `69` |  |
| PivotTableStyleDark14 | `70` |  |
| PivotTableStyleDark15 | `71` |  |
| PivotTableStyleDark16 | `72` |  |
| PivotTableStyleDark17 | `73` |  |
| PivotTableStyleDark18 | `74` |  |
| PivotTableStyleDark19 | `75` |  |
| PivotTableStyleDark20 | `76` |  |
| PivotTableStyleDark21 | `77` |  |
| PivotTableStyleDark22 | `78` |  |
| PivotTableStyleDark23 | `79` |  |
| PivotTableStyleDark24 | `80` |  |
| PivotTableStyleDark25 | `81` |  |
| PivotTableStyleDark26 | `82` |  |
| PivotTableStyleDark27 | `83` |  |
| PivotTableStyleDark28 | `84` |  |
| Custom | `85` |  |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotTableStyleTypeDemo
{
public static void PivotTableStyleTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells[0, 0].Value = "Fruit";
worksheet.Cells[0, 1].Value = "Year";
worksheet.Cells[0, 2].Value = "Amount";
worksheet.Cells[1, 0].Value = "Apple";
worksheet.Cells[1, 1].Value = 2020;
worksheet.Cells[1, 2].Value = 50;
worksheet.Cells[2, 0].Value = "Banana";
worksheet.Cells[2, 1].Value = 2020;
worksheet.Cells[2, 2].Value = 60;
worksheet.Cells[3, 0].Value = "Cherry";
worksheet.Cells[3, 1].Value = 2021;
worksheet.Cells[3, 2].Value = 70;
worksheet.Cells[4, 0].Value = "Date";
worksheet.Cells[4, 1].Value = 2021;
worksheet.Cells[4, 2].Value = 80;
// Add a pivot table to the worksheet
PivotTableCollection pivotTables = worksheet.PivotTables;
int pivotIndex = pivotTables.Add("=Sheet1!A1:C5", "E3", "PivotTable1");
PivotTable pivotTable = pivotTables[pivotIndex];
// Add fields to the pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount
// Set the pivot table style type
pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
// Save the workbook
workbook.Save("PivotTableStyleTypeExample.xlsx");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)
