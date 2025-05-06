---
title: OdsPageBackground.Color
second_title: Aspose.Cells for .NET API Reference
description: OdsPageBackground property. Gets and sets the color of background
type: docs
url: /net/aspose.cells.ods/odspagebackground/color/
---
## OdsPageBackground.Color property

Gets and sets the color of background.

```csharp
public Color Color { get; set; }
```

### Examples

```csharp
// Called: odsPageBackground.Color = Color.LightBlue;
public static void Property_Color()
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
            odsPageBackground.LinkedGraphic = &quot;path/to/graphic.png&quot;;

            // Save the workbook
            workbook.Save(&quot;OdsPageBackgroundExample.ods&quot;);
        }
```

### See Also

* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


