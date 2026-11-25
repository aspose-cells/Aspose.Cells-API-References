---
title: "ChartFrame.AutoScaleFont"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartFrame. True se il testo nell'oggetto cambia la dimensione del carattere quando la dimensione dell'oggetto cambia. Il valore predefinito è True"
type: docs
url: /it/net/aspose.cells.charts/chartframe/autoscalefont/
---
## ChartFrame.AutoScaleFont property

True se il testo nell'oggetto cambia dimensione del carattere quando le dimensioni dell'oggetto cambiano. Il valore predefinito è True.

```csharp
public virtual bool AutoScaleFont { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyAutoScaleFontDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accedi al titolo del grafico
            chart.Title.Text = "Sample Chart";
            
            // Dimostra la proprietà AutoScaleFont
            chart.Title.AutoScaleFont = true;
            Console.WriteLine("Chart title AutoScaleFont is set to: " + chart.Title.AutoScaleFont);

            // Salva la cartella di lavoro
            workbook.Save("ChartFrameAutoScaleFontDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


