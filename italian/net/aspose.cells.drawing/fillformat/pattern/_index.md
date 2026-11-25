---
title: "FillFormat.Pattern"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FillFormat. Rappresenta un modello di visualizzazione dell'area"
type: docs
url: /it/net/aspose.cells.drawing/fillformat/pattern/
---
## FillFormat.Pattern property

Rappresenta il modello di visualizzazione di un'area.

```csharp
public FillPattern Pattern { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyPatternDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue(50);
            sheet.Cells["A2"].PutValue(100);
            sheet.Cells["A3"].PutValue(150);

            // Aggiungi un grafico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = sheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("A1:A3", true);

            // Accedi alla prima serie e al suo primo punto
            ChartPoint point = chart.NSeries[0].Points[0];
            
            // Imposta il modello di riempimento per l'area del punto
            point.Area.FillFormat.Pattern = FillPattern.DottedGrid;
            
            // Salva la cartella di lavoro
            workbook.Save("FillFormatPatternDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [FillPattern](../../fillpattern/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


