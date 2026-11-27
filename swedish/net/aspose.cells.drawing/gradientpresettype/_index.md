---
title: "Enum GradientPresetType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.GradientPresetType-enum. Representerar förinställd gradientfärgstyp"
type: docs
url: /sv/net/aspose.cells.drawing/gradientpresettype/
---
## GradientPresetType enumeration

Representerar förinställd färgtyp för gradient.

```csharp
public enum GradientPresetType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Brass | `0` | Mässing förinställd färg |
| CalmWater | `1` | Lugn vatten förinställd färg |
| Chrome | `2` | Krom förinställd färg |
| ChromeII | `3` | Krom II förinställd färg |
| Daybreak | `4` | Gryning förinställd färg |
| Desert | `5` | Öken förinställd färg |
| EarlySunset | `6` | Tidigt solnedgång förinställd färg |
| Fire | `7` | Eld förinställd färg |
| Fog | `8` | Dimma förinställd färg |
| Gold | `9` | Guld förinställd färg |
| GoldII | `10` | Guld II förinställd färg |
| Horizon | `11` | Horisont förinställd färg |
| LateSunset | `12` | Sen solnedgång förinställd färg |
| Mahogany | `13` | Mahogny förinställd färg |
| Moss | `14` | Mossa förinställd färg |
| Nightfall | `15` | Skymning förinställd färg |
| Ocean | `16` | Hav förinställd färg |
| Parchment | `17` | Pergament förinställd färg |
| Peacock | `18` | Påfågel förinställd färg |
| Rainbow | `19` | Regnbåge förinställd färg |
| RainbowII | `20` | Regnbåge II förinställd färg |
| Sapphire | `21` | Safir förinställd färg |
| Silver | `22` | Silver förinställd färg |
| Wheat | `23` | Vete förinställd färg |
| Unknown | `24` | Okänd förinställd färg. Endast för den förinställda färgen (som inte är samma som någon känd förinställd färg) i mallarboken. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientPresetTypeDemo
    {
        public static void GradientPresetTypeExample()
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

            // Åtkomst till diagrammets kategoriaxel
            Axis categoryAxis = chart.CategoryAxis;

            // Åtkomst till fyllningsformatet för kategoriaxelområdet
            FillFormat fillFormat = categoryAxis.Area.FillFormat;

            // Ange en förinställd gradientfärg för fyllningsformatet
            fillFormat.SetPresetColorGradient(GradientPresetType.Fire, GradientStyleType.Horizontal, 1);

            // Skriv ut typen av förinställd gradientfärg
            Console.WriteLine("Gradient Preset Color: " + fillFormat.PresetColor);

            // Spara arbetsboken
            workbook.Save("GradientPresetTypeExample.xlsx");
            workbook.Save("GradientPresetTypeExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


