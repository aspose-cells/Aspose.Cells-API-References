---
title: "Enum BevelPresetType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.BevelPresetType enum. Representerar en förinställning för en typ av fasning som kan tillämpas på en form i 3D"
type: docs
url: /sv/net/aspose.cells.drawing/bevelpresettype/
---
## BevelPresetType enumeration

Representerar en förinställning för en typ av fasning som kan tillämpas på en form i 3D.

```csharp
public enum BevelPresetType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | Ingen avfasning |
| Angle | `1` | Vinkel |
| ArtDeco | `2` | Art deco |
| Circle | `3` | Cirkel |
| Convex | `4` | Konvex |
| CoolSlant | `5` | Cool lutning |
| Cross | `6` | Kors |
| Divot | `7` | Grop |
| HardEdge | `8` | Hård kant |
| RelaxedInset | `9` | Avslappnad infogning |
| Riblet | `10` | Ribb |
| Slope | `11` | Lutning |
| SoftRound | `12` | Mjuk rundning |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Charts;
    using System;

    public class BevelPresetTypeDemo
    {
        public static void BevelPresetTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataintervall
            chart.SetChartDataRange("A1:B4", true);

            // Kom åt diagrammets titel och ange dess text
            chart.Title.Text = "Sample Chart with Bevel";

            // Åtkomst till diagrammets plotområde
            PlotArea plotArea = chart.PlotArea;

            // Kom åt formegenskaperna för diagramområdet
            ShapePropertyCollection shapeProperties = plotArea.ShapeProperties;

            
            // Kom åt 3D-formatets egenskaper
            Format3D format3D = shapeProperties.Format3D;

            // Kom åt egenskaperna för den övre fasningen
            Bevel topBevel = format3D.TopBevel;

            // Ställ in fasningstypen till "Angle"
            topBevel.Type = BevelPresetType.Angle;

            // Ställ in bredden och höjden på fasningen
            topBevel.Width = 10;
            topBevel.Height = 10;

            // Spara arbetsboken
            workbook.Save("BevelPresetTypeExample.xlsx");
            workbook.Save("BevelPresetTypeExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


