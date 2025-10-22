##Class ConditionalFormattingIcon
Aspose.Cells.ConditionalFormattingIcon class. Represents the custom icon of conditional formatting rule
## ConditionalFormattingIcon class
Represents the custom icon of conditional formatting rule.
```csharp
public class ConditionalFormattingIcon
```
## Properties
| Name | Description |
| --- | --- |
| [ImageData](../../aspose.cells/conditionalformattingicon/imagedata/) { get; } | Gets the icon set data. |
| [Index](../../aspose.cells/conditionalformattingicon/index/) { get; set; } | Gets and sets the icon's index in the icon set. |
| [Type](../../aspose.cells/conditionalformattingicon/type/) { get; set; } | Gets and sets the icon set type. |
## Methods
| Name | Description |
| --- | --- |
| [GetImageData](../../aspose.cells/conditionalformattingicon/getimagedata/)(Cell) | Gets the image data with the setting of cell. |
| static [GetIconImageData](../../aspose.cells/conditionalformattingicon/geticonimagedata/)(IconSetType, int) | Get the icon set data |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ConditionalFormattingIconDemo
{
public static void ConditionalFormattingIconExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet in the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Get the Conditional Formattings Collection
ConditionalFormattingCollection cformattings = worksheet.ConditionalFormattings;
// Add a new conditional formatting to the collection
int index = cformattings.Add();
// Access the Format Condition Collection
FormatConditionCollection fcs = cformattings[index];
// Define the cell area to apply conditional formatting
CellArea ca = new CellArea
{
StartRow = 0,
EndRow = 10,
StartColumn = 0,
EndColumn = 0
};
// Add the cell area to the format condition collection
fcs.AddArea(ca);
// Add a condition to use icon sets
int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
FormatCondition fc = fcs[conditionIndex];
// Set the icon set type
fc.IconSet.Type = IconSetType.Arrows3;
// Customize the individual icons within the icon set
ConditionalFormattingIcon cfIcon0 = fc.IconSet.CfIcons[0];
cfIcon0.Type = IconSetType.Arrows3;
cfIcon0.Index = 0;
ConditionalFormattingIcon cfIcon1 = fc.IconSet.CfIcons[1];
cfIcon1.Type = IconSetType.ArrowsGray3;
cfIcon1.Index = 1;
ConditionalFormattingIcon cfIcon2 = fc.IconSet.CfIcons[2];
cfIcon2.Type = IconSetType.Boxes5;
cfIcon2.Index = 2;
// Save the workbook
workbook.Save("ConditionalFormattingIconExample.xlsx");
workbook.Save("ConditionalFormattingIconExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
