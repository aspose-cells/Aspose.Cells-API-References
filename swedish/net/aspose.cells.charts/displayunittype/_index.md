---
title: "Enum DisplayUnitType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.DisplayUnitType enum. Representerar typen av displayenhet för diagramaxlar"
type: docs
url: /sv/net/aspose.cells.charts/displayunittype/
---
## DisplayUnitType enumeration

Representerar typen av displayenhet för diagrammets axel.

```csharp
public enum DisplayUnitType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | Displayenhet är Ingen. |
| Hundreds | `1` | Anger att värdena i diagrammet ska divideras med 100. |
| Thousands | `2` | Anger att värdena i diagrammet ska divideras med 1 000. |
| TenThousands | `3` | Anger att värdena i diagrammet ska divideras med 10 000. |
| HundredThousands | `4` | Anger att värdena i diagrammet ska divideras med 100 000. |
| Millions | `5` | Anger att värdena i diagrammet ska divideras med 1 000 000. |
| TenMillions | `6` | Anger att värdena i diagrammet ska divideras med 10,000,000. |
| HundredMillions | `7` | Anger att värdena i diagrammet ska divideras med 100,000,000. |
| Billions | `8` | Anger att värdena i diagrammet ska divideras med 1,000,000,000. |
| Trillions | `9` | Anger att värdena i diagrammet ska divideras med 1,000,000,000,000. |
| Percentage | `10` | Värdena i diagrammet ska divideras med 0,01. |
| Cust | `11` | Anger ett anpassat värde för visningsenheten. |
| Custom | `12` | Anger ett anpassat värde för visningsenheten. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class DisplayUnitTypeDemo
    {
        public static void DisplayUnitTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett nytt kalkylblad i arbetsboken
            int sheetIndex = workbook.Worksheets.Add();
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Lägg till lite exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue(500000);
            worksheet.Cells["A2"].PutValue(1000000);
            worksheet.Cells["A3"].PutValue(1500000);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);
            
            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Lägg till NSeries (diagramdatakälla) till diagrammet som sträcker sig från cellen "A1" till "B3"
            chart.NSeries.Add("A1:B3", true);
            
            // Ställ in visningsenheten för värdeaxeln till miljoner
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Millions;
            
            // Visa eventuellt etiketten för visningsenheten
            chart.ValueAxis.IsDisplayUnitLabelShown = true;
            
            // Spara arbetsboken
            workbook.Save("DisplayUnitTypeExample.xlsx");
            workbook.Save("DisplayUnitTypeExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


