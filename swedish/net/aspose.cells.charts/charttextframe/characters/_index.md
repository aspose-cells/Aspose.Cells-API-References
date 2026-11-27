---
title: "ChartTextFrame.Characters"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartTextFrame-metod. Returnerar ett Characters-objekt som representerar ett intervall av tecken i texten"
type: docs
url: /sv/net/aspose.cells.charts/charttextframe/characters/
---
## ChartTextFrame.Characters method

Returnerar ett Characters-objekt som representerar ett intervall av tecken i texten.

```csharp
public FontSetting Characters(int startIndex, int length)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startIndex | Int32 | Indexet för början av tecknet. |
| length | Int32 | Antalet tecken. |

### Returvärde

Characters-objekt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFrameMethodCharactersWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Skapa diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Åtkomst till datamärkningar och ange teckenstorlek för specifika tecken
            chart.NSeries[0].Points[0].DataLabels.ShowValue = true;
            chart.NSeries[0].Points[0].DataLabels.Characters(0, 5).Font.Size = 14;
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


