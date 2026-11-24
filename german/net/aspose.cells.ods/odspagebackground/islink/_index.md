---
title: "OdsPageBackground.IsLink"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OdsPageBackground-Eigenschaft. Gibt an, ob es sich um eine verknüpfte Grafik handelt"
type: docs
url: /de/net/aspose.cells.ods/odspagebackground/islink/
---
## OdsPageBackground.IsLink property

Gibt an, ob es sich um eine verknüpfte Grafik handelt.

```csharp
public bool IsLink { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook(FileFormatType.Ods);
            Worksheet worksheet = workbook.Worksheets[0];

            // Zugriff auf das OdsPageBackground
            OdsPageBackground background = worksheet.PageSetup.ODSPageBackground;

            // Den aktuellen IsLink-Wert anzeigen
            Console.WriteLine("Current IsLink value: " + background.IsLink);

            // Vorhandene Hintergrund-Eigenschaften ändern, anstatt ein neues zu erstellen
            background.Type = OdsPageBackgroundType.Graphic;
            background.GraphicType = OdsPageBackgroundGraphicType.Position;
            background.GraphicPositionType = OdsPageBackgroundGraphicPositionType.TopLeft;
            background.LinkedGraphic = "path/to/image.png";

            // Den neuen IsLink-Wert anzeigen
            Console.WriteLine("New IsLink value: " + worksheet.PageSetup.ODSPageBackground.IsLink);

            // Ergebnis speichern
            workbook.Save("OdsPageBackgroundIsLinkDemo.ods");
        }
    }
}
```

### Siehe auch

* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


