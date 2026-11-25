---
title: "ChartTextFrame.IsTextWrapped"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartTextFrame. Ottiene o imposta un valore che indica se il testo è avvolto"
type: docs
url: /it/net/aspose.cells.charts/charttextframe/istextwrapped/
---
## ChartTextFrame.IsTextWrapped property

Ottiene o imposta un valore che indica se il testo è a capo.

```csharp
public virtual bool IsTextWrapped { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyIsTextWrappedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Q1");
            sheet.Cells["A3"].PutValue("Q2");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(12000);
            sheet.Cells["B3"].PutValue(15000);

            // Aggiungi grafico
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 5, 20, 10);
            Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Imposta il titolo del grafico con avvolgimento del testo
            chart.Title.Text = "Quarterly Sales Report (2023) - This is a long title that will wrap when IsTextWrapped is true";
            chart.Title.IsTextWrapped = true;
            
            // Salva cartella di lavoro
            workbook.Save("ChartTextWrappingDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


