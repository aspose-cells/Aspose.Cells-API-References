---
title: OdsPageBackground.Type
second_title: Aspose.Cells for .NET API Reference
description: OdsPageBackground property. Gets and sets the page background type
type: docs
url: /net/aspose.cells.ods/odspagebackground/type/
---
## OdsPageBackground.Type property

Gets and sets the page background type.

```csharp
public OdsPageBackgroundType Type { get; set; }
```

### Examples

```csharp
// Called: odsPageBackground.Type = OdsPageBackgroundType.Color;
public static void Property_Type()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Access the PageSetup of the worksheet
            PageSetup pageSetup = worksheet.PageSetup;

            // Access the ODSPageBackground property
            OdsPageBackground odsPageBackground = pageSetup.ODSPageBackground;

            // Set the background type to Color
            odsPageBackground.Type = OdsPageBackgroundType.Color;

            // Set the background color
            odsPageBackground.Color = Color.LightBlue;

            // Save the workbook
            workbook.Save(&quot;OdsPageBackgroundTypeExample.ods&quot;);
        }
```

### See Also

* enum [OdsPageBackgroundType](../../odspagebackgroundtype/)
* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


