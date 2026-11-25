---
title: "Enum TextureType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Drawing.TextureType. Rappresenta il tipo di trama predefinito"
type: docs
url: /it/net/aspose.cells.drawing/texturetype/
---
## TextureType enumeration

Rappresenta il tipo di texture predefinita.

```csharp
public enum TextureType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| BlueTissuePaper | `0` | Rappresenta il tipo di trama Blue Tissue Paper. |
| Bouquet | `1` | Rappresenta il tipo di trama Bouquet. |
| BrownMarble | `2` | Rappresenta il tipo di trama Brown Marble. |
| Canvas | `3` | Rappresenta il tipo di trama Canvas. |
| Cork | `4` | Rappresenta il tipo di trama Cork. |
| Denim | `5` | Rappresenta il tipo di trama Denim. |
| FishFossil | `6` | Rappresenta il tipo di trama Fish Fossil. |
| Granite | `7` | Rappresenta il tipo di trama Granite. |
| GreenMarble | `8` | Rappresenta il tipo di trama Green Marble. |
| MediumWood | `9` | Rappresenta il tipo di trama Medium Wood. |
| Newsprint | `10` | Rappresenta il tipo di trama Newsprint. |
| Oak | `11` | Rappresenta il tipo di trama Oak. |
| PaperBag | `12` | Rappresenta il tipo di trama Paper Bag. |
| Papyrus | `13` | Rappresenta il tipo di trama Papyrus. |
| Parchment | `14` | Rappresenta il tipo di trama Parchment. |
| PinkTissuePaper | `15` | Rappresenta il tipo di trama Pink Tissue Paper. |
| PurpleMesh | `16` | Rappresenta il tipo di trama Purple Mesh. |
| RecycledPaper | `17` | Rappresenta il tipo di trama Recycled Paper. |
| Sand | `18` | Rappresenta il tipo di trama Sand. |
| Stationery | `19` | Rappresenta il tipo di texture Stationery. |
| Walnut | `20` | Rappresenta il tipo di texture Walnut Droplets. |
| WaterDroplets | `21` | Rappresenta il tipo di texture Water Droplets. |
| WhiteMarble | `22` | Rappresenta il tipo di texture White Marble. |
| WovenMat | `23` | Rappresenta il tipo di texture Woven Mat. |
| Unknown | `24` | Rappresenta il tipo di texture Unknown. |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            sheet.Cells["A1"].PutValue("Item");
            sheet.Cells["A2"].PutValue("Product A");
            sheet.Cells["A3"].PutValue("Product B");
            sheet.Cells["A4"].PutValue("Product C");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["B3"].PutValue(2000);
            sheet.Cells["B4"].PutValue(3000);

            // Aggiungi un grafico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accedi alla prima serie e imposta la texture per un punto
            ChartPoint point = chart.NSeries[0].Points[2];
            point.Area.FillFormat.Texture = TextureType.Stationery;

            // Salva la cartella di lavoro
            workbook.Save("TextureTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


