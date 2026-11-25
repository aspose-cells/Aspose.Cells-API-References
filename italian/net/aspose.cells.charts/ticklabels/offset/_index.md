---
title: "TickLabels.Offset"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TickLabels. Ottiene e imposta la distanza delle etichette dall'asse di categoria. Questo si applica solo all'asse x di categoria"
type: docs
url: /it/net/aspose.cells.charts/ticklabels/offset/
---
## TickLabels.Offset property

Ottiene e imposta la distanza delle etichette dall'asse delle categorie. Questo si applica solo all'asse delle categorie (x).

```csharp
public int Offset { get; set; }
```

### Osservazioni

La distanza predefinita è del 100 percento, che rappresenta la spaziatura predefinita tra le etichette dell'asse e la linea dell'asse. Il valore può essere una percentuale intera da 0 a 1000, relativa alla dimensione del carattere dell'etichetta dell'asse.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyOffsetDemo
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
            
            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accedi all'asse dei valori
            Axis valueAxis = chart.ValueAxis;
            
            // Imposta l'offset di TickLabels
            valueAxis.TickLabels.Offset = 50; // 50% offset from default position

            // Salva la cartella di lavoro
            workbook.Save("TickLabelsOffsetDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


