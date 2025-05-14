---
title: OdsPageBackground.GraphicType
second_title: Aspose.Cells for .NET API Reference
description: OdsPageBackground property. Gets and sets the page background graphic type
type: docs
url: /net/aspose.cells.ods/odspagebackground/graphictype/
---
## OdsPageBackground.GraphicType property

Gets and sets the page background graphic type.

```csharp
public OdsPageBackgroundGraphicType GraphicType { get; set; }
```

### Examples

```csharp
// Called: odsPageBackground.GraphicType = OdsPageBackgroundGraphicType.Tile;
public static void OdsPageBackground_Property_GraphicType()
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

* enum [OdsPageBackgroundGraphicType](../../odspagebackgroundgraphictype/)
* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


