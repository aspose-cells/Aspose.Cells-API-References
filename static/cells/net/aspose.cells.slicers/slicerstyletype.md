##Enum SlicerStyleType
Aspose.Cells.Slicers.SlicerStyleType enum. Specify the style of slicer view
## SlicerStyleType enumeration
Specify the style of slicer view
```csharp
public enum SlicerStyleType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| SlicerStyleLight1 | `0` | built-in light style one |
| SlicerStyleLight2 | `1` | built-in light style two |
| SlicerStyleLight3 | `2` | built-in light style three |
| SlicerStyleLight4 | `3` | built-in light style four |
| SlicerStyleLight5 | `4` | built-in light style five |
| SlicerStyleLight6 | `5` | built-in light style six |
| SlicerStyleOther1 | `6` | built-in style other one |
| SlicerStyleOther2 | `7` | built-in style other two |
| SlicerStyleDark1 | `8` | built-in dark style one |
| SlicerStyleDark2 | `9` | built-in dark style tow |
| SlicerStyleDark3 | `10` | built-in dark style three |
| SlicerStyleDark4 | `11` | built-in dark style four |
| SlicerStyleDark5 | `12` | built-in dark style five |
| SlicerStyleDark6 | `13` | built-in dark style six |
| Custom | `14` | user-defined style, unsupported for now |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;
namespace AsposeCellsExamples
{
public class SlicersClassSlicerStyleTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
// Create sample data for pivot table
sheet.Cells["A1"].Value = "Fruit";
sheet.Cells["A2"].Value = "Apple";
sheet.Cells["A3"].Value = "Orange";
sheet.Cells["A4"].Value = "Banana";
sheet.Cells["A5"].Value = "Apple";
sheet.Cells["B1"].Value = "Quantity";
sheet.Cells["B2"].Value = 10;
sheet.Cells["B3"].Value = 15;
sheet.Cells["B4"].Value = 8;
sheet.Cells["B5"].Value = 12;
// Create pivot table
int pivotIndex = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
PivotTable pivot = sheet.PivotTables[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, 0);
pivot.AddFieldToArea(PivotFieldType.Data, 1);
// Add slicer
int slicerIndex = sheet.Slicers.Add(pivot, "G1", pivot.BaseFields[0]);
Slicer slicer = sheet.Slicers[slicerIndex];
// Set slicer style
slicer.StyleType = SlicerStyleType.SlicerStyleDark1;
slicer.NumberOfColumns = 2;
// Save the workbook
wb.Save("SlicerStyleTypeDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Slicers](../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../)
