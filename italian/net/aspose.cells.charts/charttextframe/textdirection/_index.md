---
title: "ChartTextFrame.TextDirection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartTextFrame. Rappresenta l'ordine di lettura del testo"
type: docs
url: /it/net/aspose.cells.charts/charttextframe/textdirection/
---
## ChartTextFrame.TextDirection property

Rappresenta l'ordine di lettura del testo.

```csharp
[Obsolete("Use ChartTextFrame.ReadingOrder property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public TextDirectionType TextDirection { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà ChartTextFrame.ReadingOrder. Questa proprietà sarà rimossa 12 mesi dopo, a partire da marzo 2020. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyTextDirectionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Configura i dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Configura le etichette dei dati
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            dataLabels.ShowValue = true;
            
            // Dimostra la proprietà TextDirection
            dataLabels.TextDirection = TextDirectionType.LeftToRight;

            // Salva la cartella di lavoro
            workbook.Save("ChartTextDirectionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [TextDirectionType](../../../aspose.cells/textdirectiontype/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


