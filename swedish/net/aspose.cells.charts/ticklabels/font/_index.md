---
title: "TickLabels.Font"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TickLabels‑egenskap. Returnerar ett Font‑objekt som representerar teckensnittet för det angivna TickLabels‑objektet"
type: docs
url: /sv/net/aspose.cells.charts/ticklabels/font/
---
## TickLabels.Font property

Returnerar ett `Font`‑objekt som representerar teckensnittet för det angivna TickLabels‑objektet.

```csharp
public Font Font { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyFontDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            
            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("A2:A4", true);
            chart.NSeries.CategoryData = "A1:A1";
            
            // Åtkomst till tick‑etikettens teckensnitt
            Aspose.Cells.Charts.TickLabels tickLabels = chart.CategoryAxis.TickLabels;
            Font font = tickLabels.Font;
            
            // Ställ in teckensnittsegenskaper
            font.Name = "Arial";
            font.Size = 12;
            font.IsBold = true;
            
            // Spara arbetsboken
            workbook.Save("TickLabelsFontDemo.xlsx");
            
            Console.WriteLine("TickLabels font properties set successfully.");
        }
    }
}
```

### Se även

* class [Font](../../../aspose.cells/font/)
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


