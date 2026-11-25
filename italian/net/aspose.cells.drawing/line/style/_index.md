---
title: "Line.Style"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Line. Rappresenta lo stile della linea"
type: docs
url: /it/net/aspose.cells.drawing/line/style/
---
## Line.Style property

Rappresenta lo stile della linea.

```csharp
public LineType Style { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea un grafico di esempio
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            // Ottieni la prima serie e il suo primo punto
            Series series = chart.NSeries[0];
            ChartPoint point = series.Points[0];
            
            // Imposta le proprietà della linea
            point.Border.Color = Color.Red;
            point.Border.Style = LineType.Solid;
            
            // Verifica che lo stile sia stato impostato
            Console.WriteLine("Border Style: " + point.Border.Style);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* enum [LineType](../../linetype/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


