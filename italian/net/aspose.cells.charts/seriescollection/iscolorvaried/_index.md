---
title: "SeriesCollection.IsColorVaried"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SeriesCollection. Rappresenta se il colore dei punti è variabile"
type: docs
url: /it/net/aspose.cells.charts/seriescollection/iscolorvaried/
---
## SeriesCollection.IsColorVaried property

Rappresenta se il colore dei punti è variabile.

```csharp
public bool IsColorVaried { get; set; }
```

### Osservazioni

Funziona solo per i grafici a torta o quando è presente una sola serie.

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionPropertyIsColorVariedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Dati di esempio
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Region");
            cells["A2"].PutValue("France");
            cells["A3"].PutValue("Germany");
            cells["A4"].PutValue("England");
            cells["A5"].PutValue("USA");
            cells["B1"].PutValue("Sales");
            cells["B2"].PutValue(70000);
            cells["B3"].PutValue(55000);
            cells["B4"].PutValue(30000);
            cells["B5"].PutValue(85000);

            // Crea grafico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];
            
            // Aggiungi serie
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";
            
            // Imposta la proprietà IsColorVaried
            chart.NSeries.IsColorVaried = true;
            
            // Salva la cartella di lavoro
            workbook.Save("SeriesCollectionPropertyIsColorVariedDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


