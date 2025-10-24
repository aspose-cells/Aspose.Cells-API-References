##Enum IconSetType
Aspose.Cells.IconSetType enum. Icon set type for conditional formatting. The threshold values for triggering the different icons within a set are configurable and the icon order is reversible
## IconSetType enumeration
Icon set type for conditional formatting. The threshold values for triggering the different icons within a set are configurable, and the icon order is reversible.
```csharp
public enum IconSetType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Arrows3 | `0` | 3 arrows icon set. |
| ArrowsGray3 | `1` | 3 gray arrows icon set. |
| Flags3 | `2` | 3 flags icon set. |
| Signs3 | `3` | 3 signs icon set. |
| Symbols3 | `4` | 3 symbols icon set (circled). |
| Symbols32 | `5` | 3 Symbols icon set (uncircled). |
| TrafficLights31 | `6` | 3 traffic lights icon set (unrimmed). |
| TrafficLights32 | `7` | 3 traffic lights icon set with thick black border. |
| Arrows4 | `8` | 4 arrows icon set. |
| ArrowsGray4 | `9` | 4 gray arrows icon set. |
| Rating4 | `10` | 4 ratings icon set. |
| RedToBlack4 | `11` | 4 'red to black' icon set. |
| TrafficLights4 | `12` | 4 traffic lights icon set. |
| Arrows5 | `13` | 5 arrows icon set. |
| ArrowsGray5 | `14` | 5 gray arrows icon set. |
| Quarters5 | `15` | 5 quarters icon set. |
| Rating5 | `16` | 5 rating icon set. |
| Stars3 | `17` | 3 stars set |
| Boxes5 | `18` | 5 boxes set |
| Triangles3 | `19` | 3 triangles set |
| None | `20` | None |
| CustomSet | `21` | CustomSet. This element is read-only. |
| Smilies3 | `22` | 3 smilies. Only for .ods. |
| ColorSmilies3 | `23` | 3 color smilies. Only for .ods. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsClassIconSetTypeDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
Cells cells = sheet.Cells;
// Set sample values
cells["A1"].PutValue(1);
cells["A2"].PutValue("#DIV/0!");
cells["A3"].PutValue(3);
// Add conditional formatting with icon set
ConditionalFormattingCollection cfs = sheet.ConditionalFormattings;
FormatConditionCollection fcs = cfs[cfs.Add()];
fcs.AddArea(CellArea.CreateCellArea(0, 0, 3, 0));
FormatCondition fc = fcs[fcs.AddCondition(FormatConditionType.IconSet)];
fc.IconSet.Type = IconSetType.TrafficLights31;
// Get and display results
ConditionalFormattingResult res1 = cells["A1"].GetConditionalFormattingResult();
Console.WriteLine($"A1 Icon Type: {res1.ConditionalFormattingIcon.Type}, Index: {res1.ConditionalFormattingIcon.Index}");
ConditionalFormattingResult res3 = cells["A3"].GetConditionalFormattingResult();
Console.WriteLine($"A3 Icon Type: {res3.ConditionalFormattingIcon.Type}, Index: {res3.ConditionalFormattingIcon.Index}");
ConditionalFormattingResult res2 = cells["A2"].GetConditionalFormattingResult();
Console.WriteLine($"A2 has formatting: {res2 != null && res2.ConditionalFormattingIcon != null}");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
