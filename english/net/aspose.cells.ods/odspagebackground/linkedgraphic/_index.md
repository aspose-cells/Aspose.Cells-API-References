---
title: OdsPageBackground.LinkedGraphic
second_title: Aspose.Cells for .NET API Reference
description: OdsPageBackground property. Gets and sets the linked graphic path
type: docs
url: /net/aspose.cells.ods/odspagebackground/linkedgraphic/
---
## OdsPageBackground.LinkedGraphic property

Gets and sets the linked graphic path.

```csharp
public string LinkedGraphic { get; set; }
```

### Examples

```csharp
// Called: odsPageBackground.LinkedGraphic = &amp;quot;background_image.png&amp;quot;;
public static void Property_LinkedGraphic()
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
            odsPageBackground.LinkedGraphic = &quot;background_image.png&quot;;

            // Save the workbook
            workbook.Save(&quot;OdsPageBackgroundGraphicTypeExample.ods&quot;);
        }
```

### See Also

* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


