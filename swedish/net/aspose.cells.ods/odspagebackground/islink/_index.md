---
title: "OdsPageBackground.IsLink"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OdsPageBackground-egenskap. Anger om det är en länkad grafik"
type: docs
url: /sv/net/aspose.cells.ods/odspagebackground/islink/
---
## OdsPageBackground.IsLink property

Indikerar om det är en länkad grafik.

```csharp
public bool IsLink { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;

    public class OdsPageBackgroundPropertyIsLinkDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook(FileFormatType.Ods);
            Worksheet worksheet = workbook.Worksheets[0];

            // Åtkomst till OdsPageBackground
            OdsPageBackground background = worksheet.PageSetup.ODSPageBackground;

            // Visa det aktuella IsLink‑värdet
            Console.WriteLine("Current IsLink value: " + background.IsLink);

            // Ändra befintliga bakgrundsegenskaper istället för att skapa en ny
            background.Type = OdsPageBackgroundType.Graphic;
            background.GraphicType = OdsPageBackgroundGraphicType.Position;
            background.GraphicPositionType = OdsPageBackgroundGraphicPositionType.TopLeft;
            background.LinkedGraphic = "path/to/image.png";

            // Visa det nya IsLink‑värdet
            Console.WriteLine("New IsLink value: " + worksheet.PageSetup.ODSPageBackground.IsLink);

            // Spara resultatet
            workbook.Save("OdsPageBackgroundIsLinkDemo.ods");
        }
    }
}
```

### Se även

* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


