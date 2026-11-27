---
title: "Enum TextureType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.TextureType‑enum. Representerar den förinställda texturtypen"
type: docs
url: /sv/net/aspose.cells.drawing/texturetype/
---
## TextureType enumeration

Representerar den förinställda texturtypen.

```csharp
public enum TextureType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| BlueTissuePaper | `0` | Representerar blått tissue‑pappers‑texturtyp. |
| Bouquet | `1` | Representerar bukett‑texturtyp. |
| BrownMarble | `2` | Representerar brun marmor‑texturtyp. |
| Canvas | `3` | Representerar canvas‑texturtyp. |
| Cork | `4` | Representerar kork‑texturtyp. |
| Denim | `5` | Representerar denimtexturtyp. |
| FishFossil | `6` | Representerar fiskfossiltexturtyp. |
| Granite | `7` | Representerar granittexturtyp. |
| GreenMarble | `8` | Representerar grön marmortexturtyp. |
| MediumWood | `9` | Representerar medelträtexturtyp. |
| Newsprint | `10` | Representerar tidningspapperstexturtyp. |
| Oak | `11` | Representerar ektexturtyp. |
| PaperBag | `12` | Representerar papperspåsetexturtyp. |
| Papyrus | `13` | Representerar papyrustexturtyp. |
| Parchment | `14` | Representerar pergamenttexturtyp. |
| PinkTissuePaper | `15` | Representerar rosa tissuepapperstexturtyp. |
| PurpleMesh | `16` | Representerar lila nättexturtyp. |
| RecycledPaper | `17` | Representerar återvunnet papperstexturtyp. |
| Sand | `18` | Representerar sandtexturtyp. |
| Stationery | `19` | Representerar kontorsmaterialtexturtyp. |
| Walnut | `20` | Representerar valnötsdroppstexturtyp. |
| WaterDroplets | `21` | Representerar vattendroppstexturtyp. |
| WhiteMarble | `22` | Representerar vit marmortexturtyp. |
| WovenMat | `23` | Representerar vävd mattetexturtyp. |
| Unknown | `24` | Representerar okänd texturtyp. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            sheet.Cells["A1"].PutValue("Item");
            sheet.Cells["A2"].PutValue("Product A");
            sheet.Cells["A3"].PutValue("Product B");
            sheet.Cells["A4"].PutValue("Product C");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["B3"].PutValue(2000);
            sheet.Cells["B4"].PutValue(3000);

            // Lägg till ett diagram
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Få åtkomst till den första serien och ange textur för en punkt
            ChartPoint point = chart.NSeries[0].Points[2];
            point.Area.FillFormat.Texture = TextureType.Stationery;

            // Spara arbetsboken
            workbook.Save("TextureTypeDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


