---
title: "ChartTextFrame.LinkedSource"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartTextFrame. Ottiene e imposta un riferimento al foglio di lavoro"
type: docs
url: /it/net/aspose.cells.charts/charttextframe/linkedsource/
---
## ChartTextFrame.LinkedSource property

Ottiene e imposta un riferimento al foglio di lavoro.

```csharp
public virtual string LinkedSource { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyLinkedSourceDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["P1"].PutValue("Chart Title");
            
            // Aggiungi grafico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta il titolo del grafico e collegalo alla cella P1
            chart.Title.Text = "Linked Title";
            chart.Title.LinkedSource = "='" + worksheet.Name + "'!$P$1";
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
            
            // Verifica la fonte collegata
            Console.WriteLine("Chart Title Linked Source: " + chart.Title.LinkedSource);
        }
    }
}
```

### Vedi anche

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


