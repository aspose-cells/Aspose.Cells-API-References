##Enum OdsPageBackgroundGraphicPositionType
Aspose.Cells.Ods.OdsPageBackgroundGraphicPositionType enum. Represents the position
## OdsPageBackgroundGraphicPositionType enumeration
Represents the position.
```csharp
public enum OdsPageBackgroundGraphicPositionType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| TopLeft | `0` | Top left. |
| TopCenter | `1` | Top center. |
| TopRight | `2` | Top right. |
| CenterLeft | `3` | Center left. |
| CenterCenter | `4` | Center. |
| CenterRight | `5` | Center right. |
| BottomLeft | `6` | Bottom left. |
| BottomCenter | `7` | Bottom center. |
| BottomRight | `8` | Bottom right. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;
using System.Drawing;
namespace AsposeCellsExamples
{
public class OdsClassOdsPageBackgroundGraphicPositionTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
PageSetup pageSetup = sheet.PageSetup;
OdsPageBackground odsPageBackground = pageSetup.ODSPageBackground;
odsPageBackground.Type = OdsPageBackgroundType.Color;
odsPageBackground.Color = Color.LightBlue;
odsPageBackground.GraphicType = OdsPageBackgroundGraphicType.Tile;
odsPageBackground.GraphicPositionType = OdsPageBackgroundGraphicPositionType.CenterCenter;
workbook.Save("OdsPageBackgroundExample.ods");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)
