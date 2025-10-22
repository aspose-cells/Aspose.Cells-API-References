##Class IconSet
Aspose.Cells.IconSet class. Describe the IconSet conditional formatting rule. This conditional formatting rule applies icons to cells according to their values
## IconSet class
Describe the IconSet conditional formatting rule. This conditional formatting rule applies icons to cells according to their values.
```csharp
public class IconSet
```
## Properties
| Name | Description |
| --- | --- |
| [CfIcons](../../aspose.cells/iconset/cficons/) { get; } | Get the[`ConditionalFormattingIcon`](../conditionalformattingicon/) from the collection |
| [Cfvos](../../aspose.cells/iconset/cfvos/) { get; } | Get the CFValueObjects instance. |
| [IsCustom](../../aspose.cells/iconset/iscustom/) { get; } | Indicates whether the icon set is custom. Default value is false. |
| [Reverse](../../aspose.cells/iconset/reverse/) { get; set; } | Get or set the flag indicating whether to reverses the default order of the icons in this icon set. Default value is false. |
| [ShowValue](../../aspose.cells/iconset/showvalue/) { get; set; } | Get or set the flag indicating whether to show the values of the cells on which this icon set is applied. Default value is true. |
| [Type](../../aspose.cells/iconset/type/) { get; set; } | Get or Set the icon set type to display. Setting the type will auto check if the current Cfvos's count is accord with the new type. If not accord, old Cfvos will be cleaned and default Cfvos will be added. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class IconSetDemo
{
public static void IconSetExample()
{
// Instantiating a Workbook object
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Adds an empty conditional formatting
int index = sheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
// Sets the conditional format range
CellArea ca = new CellArea
{
StartRow = 0,
EndRow = 2,
StartColumn = 0,
EndColumn = 0
};
fcs.AddArea(ca);
// Adds condition
int idx = fcs.AddCondition(FormatConditionType.IconSet);
FormatCondition cond = fcs[idx];
// Get Icon Set
IconSet iconSet = cond.IconSet;
// Set Icon Type
iconSet.Type = IconSetType.Arrows3;
// Set additional properties
iconSet.ShowValue = true;
iconSet.Reverse = false;
// Put Cell Values
sheet.Cells["A1"].PutValue(10);
sheet.Cells["A2"].PutValue(120);
sheet.Cells["A3"].PutValue(260);
// Saving the Excel file
workbook.Save("IconSetExample.xlsx");
workbook.Save("IconSetExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
