---
title: "Klasse OdsPageBackground"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Ods.OdsPageBackground Klasse. Stellt den Seitenhintergrund von ods dar"
type: docs
url: /de/net/aspose.cells.ods/odspagebackground/
---
## OdsPageBackground class

Stellt den Seitenhintergrund von ODS dar.

```csharp
public class OdsPageBackground
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [OdsPageBackground](odspagebackground/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Color](../../aspose.cells.ods/odspagebackground/color/) { get; set; } | Liest und setzt die Farbe des Hintergrunds. |
| [GraphicData](../../aspose.cells.ods/odspagebackground/graphicdata/) { get; set; } | Liest und setzt die Grafikdaten. |
| [GraphicPositionType](../../aspose.cells.ods/odspagebackground/graphicpositiontype/) { get; set; } | Liest und setzt die Position der Hintergrundgrafik. |
| [GraphicType](../../aspose.cells.ods/odspagebackground/graphictype/) { get; set; } | Liest und setzt den Typ der Seitenhintergrundgrafik. |
| [IsLink](../../aspose.cells.ods/odspagebackground/islink/) { get; } | Gibt an, ob es sich um eine verknüpfte Grafik handelt. |
| [LinkedGraphic](../../aspose.cells.ods/odspagebackground/linkedgraphic/) { get; set; } | Liest und setzt den Pfad der verknüpften Grafik. |
| [Type](../../aspose.cells.ods/odspagebackground/type/) { get; set; } | Liest und setzt den Seitenhintergrundtyp. |

### Beispiele

```csharp
using Aspose.Cells;
using Aspose.Cells.Ods;
using System;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class OdsPageBackgroundDemo
    {
        public static void OdsPageBackgroundExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Greifen Sie auf das PageSetup-Objekt zu
            PageSetup pageSetup = sheet.PageSetup;

            // Greife auf das ODSPageBackground-Objekt zu
            OdsPageBackground odsPageBackground = pageSetup.ODSPageBackground;

            // Setze den Hintergrundtyp auf Farbe
            odsPageBackground.Type = OdsPageBackgroundType.Color;

            // Legen Sie die Hintergrundfarbe fest
            odsPageBackground.Color = Color.LightBlue;

            // Setze den Typ der Hintergrundgrafik
            odsPageBackground.GraphicType = OdsPageBackgroundGraphicType.Tile;

            // Setze die Position der Hintergrundgrafik
            odsPageBackground.GraphicPositionType = OdsPageBackgroundGraphicPositionType.CenterCenter;

            // Setze den Pfad der verknüpften Grafik (falls vorhanden)
            odsPageBackground.LinkedGraphic = "path/to/graphic.png";

            // Speichere die Arbeitsmappe
            workbook.Save("OdsPageBackgroundExample.ods");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


