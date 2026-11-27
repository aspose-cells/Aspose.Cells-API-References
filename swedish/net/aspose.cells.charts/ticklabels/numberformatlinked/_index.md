---
title: "TickLabels.NumberFormatLinked"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TickLabels‑egenskap. Sant om talformatet är länkat till cellerna så att talformatet ändras i etiketterna när det ändras i cellerna"
type: docs
url: /sv/net/aspose.cells.charts/ticklabels/numberformatlinked/
---
## TickLabels.NumberFormatLinked property

Sant om talformatet är länkat till cellerna (så att talformatet ändras i etiketterna när det ändras i cellerna).

```csharp
public bool NumberFormatLinked { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyNumberFormatLinkedDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(100);
            worksheet.Cells["A2"].PutValue(200);
            worksheet.Cells["A3"].PutValue(300);
            worksheet.Cells["A4"].PutValue(400);
            
            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("A1:A4", true);
            
            // Få åtkomst till värdeaxelns tick‑etiketter
            Aspose.Cells.Charts.TickLabels tickLabels = chart.ValueAxis.TickLabels;
            
            // Demonstrera NumberFormatLinked‑egenskapen
            Console.WriteLine("NumberFormatLinked (default): " + tickLabels.NumberFormatLinked);
            
            // Ändra egenskapen
            tickLabels.NumberFormatLinked = false;
            Console.WriteLine("NumberFormatLinked after change: " + tickLabels.NumberFormatLinked);
            
            // Spara arbetsboken
            workbook.Save("TickLabelsNumberFormatLinkedDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


