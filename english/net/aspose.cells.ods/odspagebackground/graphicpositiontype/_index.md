---
title: OdsPageBackground.GraphicPositionType
second_title: Aspose.Cells for .NET API Reference
description: OdsPageBackground property. Gets and set the background graphic position
type: docs
url: /net/aspose.cells.ods/odspagebackground/graphicpositiontype/
---
## OdsPageBackground.GraphicPositionType property

Gets and set the background graphic position.

```csharp
public OdsPageBackgroundGraphicPositionType GraphicPositionType { get; set; }
```

### Examples

```csharp
// Called: odsPageBackground.GraphicPositionType = OdsPageBackgroundGraphicPositionType.CenterCenter;
public static void OdsPageBackground_Property_GraphicPositionType()
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

* enum [OdsPageBackgroundGraphicPositionType](../../odspagebackgroundgraphicpositiontype/)
* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


