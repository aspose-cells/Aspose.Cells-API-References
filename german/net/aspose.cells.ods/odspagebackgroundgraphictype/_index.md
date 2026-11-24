---
title: "Enum OdsPageBackgroundGraphicType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Ods.OdsPageBackgroundGraphicType enum. Stellt den Typ der Formatierung des Seitenhintergrunds mit Bild dar"
type: docs
url: /de/net/aspose.cells.ods/odspagebackgroundgraphictype/
---
## OdsPageBackgroundGraphicType enumeration

Stellt den Typ der Formatierung des Seitenhintergrunds mit Bild dar.

```csharp
public enum OdsPageBackgroundGraphicType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Position | `0` | Legen Sie das Bild an einer bestimmten Position fest. |
| Area | `1` | Strecken Sie das Bild. |
| Tile | `2` | Wiederholen Sie das Bild. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;
    using System.Drawing;

    public class OdsPageBackgroundGraphicTypeDemo
    {
        public static void OdsPageBackgroundGraphicTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];

            // Zugriff auf die Seiteneinrichtung des Arbeitsblatts
            PageSetup pageSetup = worksheet.PageSetup;

            // Greifen Sie auf das ODSPageBackground des PageSetup zu
            OdsPageBackground odsPageBackground = pageSetup.ODSPageBackground;

            // Legen Sie die Hintergrundfarbe fest
            odsPageBackground.Color = Color.LightBlue;

            // Setzen Sie den Hintergrundgrafiktyp auf Kachel
            odsPageBackground.GraphicType = OdsPageBackgroundGraphicType.Tile;

            // Setzen Sie den Pfad zur verknüpften Grafik (unter der Annahme, dass das Bild im selben Verzeichnis wie die ausführbare Datei liegt)
            odsPageBackground.LinkedGraphic = "background_image.png";

            // Speichere die Arbeitsmappe
            workbook.Save("OdsPageBackgroundGraphicTypeExample.ods");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


