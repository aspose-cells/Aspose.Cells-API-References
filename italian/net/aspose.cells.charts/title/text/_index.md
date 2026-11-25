---
title: "Title.Text"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Title. Ottiene o imposta il testo dell'etichetta dell'unità di visualizzazione"
type: docs
url: /it/net/aspose.cells.charts/title/text/
---
## Title.Text property

Ottiene o imposta il testo dell'etichetta dell'unità di visualizzazione.

```csharp
public override string Text { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TitlePropertyTextDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro e aggiungi dati di esempio
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Q1");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(200);
            worksheet.Cells["A4"].PutValue(300);
            
            // Aggiungi un grafico e imposta il testo del titolo dell'asse dei valori
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.ValueAxis.Title.Text = "Sales Amount";
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


