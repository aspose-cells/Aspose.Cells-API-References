---
title: Enum OdsPageBackgroundGraphicPositionType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Ods.OdsPageBackgroundGraphicPositionType enum. Represents the position
type: docs
url: /net/aspose.cells.ods/odspagebackgroundgraphicpositiontype/
---
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
// Called: odsPageBackground.GraphicPositionType = OdsPageBackgroundGraphicPositionType.CenterCenter;
public static void Type_OdsPageBackgroundGraphicPositionType()
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
```

### See Also

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


