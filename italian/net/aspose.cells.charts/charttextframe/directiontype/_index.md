---
title: "ChartTextFrame.DirectionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartTextFrame. Ottiene e imposta la direzione del testo"
type: docs
url: /it/net/aspose.cells.charts/charttextframe/directiontype/
---
## ChartTextFrame.DirectionType property

Ottiene e imposta la direzione del testo.

```csharp
public virtual ChartTextDirectionType DirectionType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyDirectionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            // L'aggiunta di un foglio di lavoro restituisce il suo indice, quindi otteniamo il foglio di lavoro per indice
            int sheetIndex = workbook.Worksheets.Add();
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Q3");

            // Aggiungi grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);
            chart.NSeries.CategoryData = "C1:C3";

            // Accedi e configura il titolo
            ChartTextFrame title = chart.Title;
            title.Text = "Sample Chart";
            
            // Dimostra la proprietà DirectionType
            title.DirectionType = ChartTextDirectionType.Vertical;
            
            // Salva la cartella di lavoro
            workbook.Save("ChartTextDirectionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ChartTextDirectionType](../../charttextdirectiontype/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


