##Class OdsPageBackground
Aspose.Cells.Ods.OdsPageBackground class. Represents the page background of ods
## OdsPageBackground class
Represents the page background of ods.
```csharp
public class OdsPageBackground
```
## Constructors
| Name | Description |
| --- | --- |
| [OdsPageBackground](odspagebackground/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [Color](../../aspose.cells.ods/odspagebackground/color/) { get; set; } | Gets and sets the color of background. |
| [GraphicData](../../aspose.cells.ods/odspagebackground/graphicdata/) { get; set; } | Gets and sets the graphic data. |
| [GraphicPositionType](../../aspose.cells.ods/odspagebackground/graphicpositiontype/) { get; set; } | Gets and set the background graphic position. |
| [GraphicType](../../aspose.cells.ods/odspagebackground/graphictype/) { get; set; } | Gets and sets the page background graphic type. |
| [IsLink](../../aspose.cells.ods/odspagebackground/islink/) { get; } | Indicates whether it's a linked graphic. |
| [LinkedGraphic](../../aspose.cells.ods/odspagebackground/linkedgraphic/) { get; set; } | Gets and sets the linked graphic path. |
| [Type](../../aspose.cells.ods/odspagebackground/type/) { get; set; } | Gets and sets the page background type. |
### Examples
```csharp
using Aspose.Cells;
using Aspose.Cells.Ods;
using System;
using System.Drawing;
namespace AsposeCellsExamples
{
public class OdsPageBackgroundDemo
{
public static void OdsPageBackgroundExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Access the PageSetup object
PageSetup pageSetup = sheet.PageSetup;
// Access the ODSPageBackground object
OdsPageBackground odsPageBackground = pageSetup.ODSPageBackground;
// Set the background type to Color
odsPageBackground.Type = OdsPageBackgroundType.Color;
// Set the background color
odsPageBackground.Color = Color.LightBlue;
// Set the background graphic type
odsPageBackground.GraphicType = OdsPageBackgroundGraphicType.Tile;
// Set the background graphic position
odsPageBackground.GraphicPositionType = OdsPageBackgroundGraphicPositionType.CenterCenter;
// Set the linked graphic path (if any)
odsPageBackground.LinkedGraphic = "path/to/graphic.png";
// Save the workbook
workbook.Save("OdsPageBackgroundExample.ods");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)
