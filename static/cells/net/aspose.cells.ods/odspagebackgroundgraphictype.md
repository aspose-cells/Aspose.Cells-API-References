##Enum OdsPageBackgroundGraphicType
Aspose.Cells.Ods.OdsPageBackgroundGraphicType enum. Represents the type of formatting page background with image
## OdsPageBackgroundGraphicType enumeration
Represents the type of formatting page background with image.
```csharp
public enum OdsPageBackgroundGraphicType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Position | `0` | Set the image at specific position. |
| Area | `1` | Stretch the image. |
| Tile | `2` | Repeat and repeat the image. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Ods;
using System;
using System.Drawing;
public class OdsPageBackgroundGraphicTypeDemo
{
public static void OdsPageBackgroundGraphicTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Access the PageSetup of the worksheet
PageSetup pageSetup = worksheet.PageSetup;
// Access the ODSPageBackground of the PageSetup
OdsPageBackground odsPageBackground = pageSetup.ODSPageBackground;
// Set the background color
odsPageBackground.Color = Color.LightBlue;
// Set the background graphic type to Tile
odsPageBackground.GraphicType = OdsPageBackgroundGraphicType.Tile;
// Set the linked graphic path (assuming the image is in the same directory as the executable)
odsPageBackground.LinkedGraphic = "background_image.png";
// Save the workbook
workbook.Save("OdsPageBackgroundGraphicTypeExample.ods");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)
