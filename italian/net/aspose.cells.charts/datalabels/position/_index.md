---
title: "DataLabels.Position"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataLabels. Rappresenta la posizione dell'etichetta dati"
type: docs
url: /it/net/aspose.cells.charts/datalabels/position/
---
## DataLabels.Position property

Rappresenta la posizione dell'etichetta dati.

```csharp
public LabelPositionType Position { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyPositionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Abilita le etichette dei dati
            chart.NSeries[0].DataLabels.ShowValue = true;
            
            // Imposta la posizione dell'etichetta dati
            chart.NSeries[0].DataLabels.Position = LabelPositionType.Right;

            // Salva la cartella di lavoro
            workbook.Save("DataLabelsPositionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [LabelPositionType](../../labelpositiontype/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


