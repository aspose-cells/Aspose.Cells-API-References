---
title: "Line.BeginType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Line. Specifica una punta di freccia per l'inizio di una linea"
type: docs
url: /it/net/aspose.cells.drawing/line/begintype/
---
## Line.BeginType property

Specifica una punta di freccia per l'inizio di una linea.

```csharp
public MsoArrowheadStyle BeginType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyBeginTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Aggiungi un grafico a linee
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta la fonte dati del grafico
            chart.NSeries.Add("A1:A3", true);

            // Ottieni la prima serie e configura le sue proprietà di linea
            Series series = chart.NSeries[0];
            series.Border.BeginType = MsoArrowheadStyle.Arrow;
            series.Border.EndType = MsoArrowheadStyle.ArrowDiamond;
            series.Border.Color = Color.Red;
            series.Border.Weight = WeightType.MediumLine;

            // Salva la cartella di lavoro
            workbook.Save("LinePropertyBeginTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [MsoArrowheadStyle](../../msoarrowheadstyle/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


