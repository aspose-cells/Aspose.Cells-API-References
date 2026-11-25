---
title: "ChartTextFrame.Text"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartTextFrame. Ottiene o imposta il testo del titolo di un frame"
type: docs
url: /it/net/aspose.cells.charts/charttextframe/text/
---
## ChartTextFrame.Text property

Ottiene o imposta il testo del titolo di un frame.

```csharp
public virtual string Text { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyTextDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Category");
            cells["A2"].PutValue("A");
            cells["A3"].PutValue("B");
            cells["A4"].PutValue("C");
            cells["B1"].PutValue("Value");
            cells["B2"].PutValue(10);
            cells["B3"].PutValue(20);
            cells["B4"].PutValue(30);

            // Aggiungi grafico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Imposta il testo del titolo del grafico
            chart.Title.Text = "Sample Chart Title";

            // Accedi e modifica il testo della legenda
            Legend legend = chart.Legend;
            legend.Text = "Custom Legend Text";

            // Salva la cartella di lavoro
            workbook.Save("ChartTextDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


