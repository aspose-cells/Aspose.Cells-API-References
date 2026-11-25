---
title: "TickLabels.RotationAngle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TickLabels. Rappresenta l'angolo di rotazione del testo in senso orario"
type: docs
url: /it/net/aspose.cells.charts/ticklabels/rotationangle/
---
## TickLabels.RotationAngle property

Rappresenta l'angolo di rotazione del testo in senso orario.

```csharp
public int RotationAngle { get; set; }
```

### Osservazioni

0: Non ruotato.255: Dall'alto al basso.-90: Verso il basso.90: Verso l'alto.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyRotationAngleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue("Category 1");
            sheet.Cells["A2"].PutValue("Category 2");
            sheet.Cells["A3"].PutValue("Category 3");
            sheet.Cells["B1"].PutValue(100);
            sheet.Cells["B2"].PutValue(200);
            sheet.Cells["B3"].PutValue(300);

            // Aggiungi un grafico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];
            
            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Ruota le etichette dei tick dell'asse di categoria di 45 gradi
            chart.CategoryAxis.TickLabels.RotationAngle = 45;

            // Salva la cartella di lavoro
            workbook.Save("TickLabelsRotationDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


