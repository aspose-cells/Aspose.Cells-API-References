---
title: "Line.EndArrowWidth"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Line. Specifica la larghezza della punta della freccia per la fine di una linea"
type: docs
url: /it/net/aspose.cells.drawing/line/endarrowwidth/
---
## Line.EndArrowWidth property

Specifica la larghezza della punta della freccia per la fine di una linea.

```csharp
public MsoArrowheadWidth EndArrowWidth { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LinePropertyEndArrowWidthDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per il grafico a linee
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["B3"].PutValue(6);

            // Aggiungi un grafico a linee
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta la fonte dati del grafico
            chart.NSeries.Add("A1:B3", true);

            // Configura le proprietà della linea per la prima serie
            Series series = chart.NSeries[0];
            series.Border.EndArrowWidth = MsoArrowheadWidth.Wide;
            series.Border.EndType = MsoArrowheadStyle.Arrow;

            // Salva la cartella di lavoro
            workbook.Save("LinePropertyEndArrowWidthDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [MsoArrowheadWidth](../../msoarrowheadwidth/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


