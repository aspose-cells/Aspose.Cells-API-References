##IconSet.Type
IconSet property. Get or Set the icon set type to display. Setting the type will auto check if the current Cfvoss count is accord with the new type. If not accord old Cfvos will be cleaned and default Cfvos will be added
## IconSet.Type property
Get or Set the icon set type to display. Setting the type will auto check if the current Cfvos's count is accord with the new type. If not accord, old Cfvos will be cleaned and default Cfvos will be added.
```csharp
public IconSetType Type { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class IconSetPropertyTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
int index = sheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
CellArea ca = new CellArea
{
StartRow = 0,
EndRow = 2,
StartColumn = 0,
EndColumn = 0
};
fcs.AddArea(ca);
int idx = fcs.AddCondition(FormatConditionType.IconSet);
FormatCondition cond = fcs[idx];
IconSet iconSet = cond.IconSet;
// Demonstrate Type property usage
iconSet.Type = IconSetType.Arrows3;
sheet.Cells["A1"].PutValue(10);
sheet.Cells["A2"].PutValue(120);
sheet.Cells["A3"].PutValue(260);
workbook.Save("IconSetExample.xlsx");
}
}
}
```
### See Also
* enum [IconSetType](../../iconsettype/)
* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
