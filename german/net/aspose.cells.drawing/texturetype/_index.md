---
title: "Enum TextureType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.TextureType enum. Stellt den vordefinierten Texturtyp dar"
type: docs
url: /de/net/aspose.cells.drawing/texturetype/
---
## TextureType enumeration

Stellt den voreingestellten Texturtyp dar.

```csharp
public enum TextureType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| BlueTissuePaper | `0` | Stellt den Texturtyp Blue Tissue Paper dar. |
| Bouquet | `1` | Stellt den Texturtyp Bouquet dar. |
| BrownMarble | `2` | Stellt den Texturtyp Brown Marble dar. |
| Canvas | `3` | Stellt den Texturtyp Canvas dar. |
| Cork | `4` | Stellt den Texturtyp Cork dar. |
| Denim | `5` | Stellt den Texturtyp Denim dar. |
| FishFossil | `6` | Stellt den Texturtyp Fish Fossil dar. |
| Granite | `7` | Stellt den Texturtyp Granite dar. |
| GreenMarble | `8` | Stellt den Texturtyp Grün Marmor dar. |
| MediumWood | `9` | Stellt den Texturtyp Mittleres Holz dar. |
| Newsprint | `10` | Stellt den Texturtyp Zeitungspapier dar. |
| Oak | `11` | Stellt den Texturtyp Eiche dar. |
| PaperBag | `12` | Stellt den Texturtyp Papiertüte dar. |
| Papyrus | `13` | Stellt den Texturtyp Papyrus dar. |
| Parchment | `14` | Stellt den Texturtyp Pergament dar. |
| PinkTissuePaper | `15` | Stellt den Texturtyp Rosa Taschentuchpapier dar. |
| PurpleMesh | `16` | Stellt den Texturtyp Lila Netz dar. |
| RecycledPaper | `17` | Stellt den Texturtyp Recyclingpapier dar. |
| Sand | `18` | Stellt den Texturtyp Sand dar. |
| Stationery | `19` | Stellt den Texturtyp Schreibwaren dar. |
| Walnut | `20` | Stellt den Texturtyp Walnusströpfchen dar. |
| WaterDroplets | `21` | Stellt den Texturtyp Wassertropfen dar. |
| WhiteMarble | `22` | Stellt den Texturtyp Weißer Marmor dar. |
| WovenMat | `23` | Stellt den Texturtyp Gewebte Matte dar. |
| Unknown | `24` | Stellt den unbekannten Texturtyp dar. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassTextureTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Beispieldaten zum Diagramm hinzufügen
            sheet.Cells["A1"].PutValue("Item");
            sheet.Cells["A2"].PutValue("Product A");
            sheet.Cells["A3"].PutValue("Product B");
            sheet.Cells["A4"].PutValue("Product C");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["B3"].PutValue(2000);
            sheet.Cells["B4"].PutValue(3000);

            // Füge ein Diagramm hinzu
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Greifen Sie auf die erste Serie zu und setzen Sie die Textur für einen Punkt
            ChartPoint point = chart.NSeries[0].Points[2];
            point.Area.FillFormat.Texture = TextureType.Stationery;

            // Speichere die Arbeitsmappe
            workbook.Save("TextureTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


