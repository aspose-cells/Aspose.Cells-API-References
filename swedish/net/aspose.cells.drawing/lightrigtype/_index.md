---
title: "Enum LightRigType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.LightRigType enum. Representerar en förinställd ljusriktning som kan tillämpas på en form"
type: docs
url: /sv/net/aspose.cells.drawing/lightrigtype/
---
## LightRigType enumeration

Representerar en förinställd ljusrättning som kan tillämpas på en form.

```csharp
public enum LightRigType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Balanced | `0` | Balanserad |
| BrightRoom | `1` | Ljust rum |
| Chilly | `2` | Kylig |
| Contrasting | `3` | Kontrasterande |
| Flat | `4` | Platt |
| Flood | `5` | Flod |
| Freezing | `6` | Frysande |
| Glow | `7` | Glöd |
| Harsh | `8` | Skarp |
| LegacyFlat1 | `9` | LegacyFlat1 |
| LegacyFlat2 | `10` | LegacyFlat2 |
| LegacyFlat3 | `11` | LegacyFlat3 |
| LegacyFlat4 | `12` | LegacyFlat4 |
| LegacyHarsh1 | `13` | LegacyHarsh1 |
| LegacyHarsh2 | `14` | LegacyHarsh2 |
| LegacyHarsh3 | `15` | LegacyHarsh3 |
| LegacyHarsh4 | `16` | LegacyHarsh4 |
| LegacyNormal1 | `17` | LegacyNormal1 |
| LegacyNormal2 | `18` | LegacyNormal2 |
| LegacyNormal3 | `19` | LegacyNormal3 |
| LegacyNormal4 | `20` | LegacyNormal4 |
| Morning | `21` | Morgon |
| Soft | `22` | Mjuk |
| Sunrise | `23` | Soluppgång |
| Sunset | `24` | Solnedgång |
| ThreePoint | `25` | Tre punkter |
| TwoPoint | `26` | Två punkter |
| None | `27` | Ingen ljusrigg. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class LightRigTypeDemo
    {
        public static void LightRigTypeExample()
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataintervall
            chart.SetChartDataRange("A1:B4", true);

            // Få åtkomst till den första serien i diagrammet
            Series series = chart.NSeries[0];

            // Åtkomst till formegenskaperna för serien
            ShapePropertyCollection shapeProperties = series.ShapeProperties;

            // Kontrollera om serien har 3D-formatdata
            if (shapeProperties.HasFormat3D())
            {
                // Kom åt 3D-formatets egenskaper
                Format3D format3D = shapeProperties.Format3D;

                // Ställ in ytliga belysningstyp till Balanced
                format3D.SurfaceLightingType = LightRigType.Balanced;

                // Ställ in belysningsvinkeln
                format3D.LightingAngle = 45.0;
            }

            // Spara arbetsboken
            workbook.Save("LightRigTypeExample.xlsx");
            workbook.Save("LightRigTypeExample.pdf");
            // Skriv ut resultaten
            Console.WriteLine("LightRigType example applied and workbook saved as 'LightRigTypeExample.xlsx'.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


