---
title: "ChartArea.Height"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartArea. Ottiene o imposta lo spostamento verticale dalla riga dell'angolo inferiore destro in unità di 1/4000 dell'area del grafico"
type: docs
url: /it/net/aspose.cells.charts/chartarea/height/
---
## ChartArea.Height property

Ottiene o imposta lo spostamento verticale dalla riga dell'angolo inferiore‑destro, in unità di 1/4000 dell'area del grafico.

```csharp
[Obsolete("Use ChartArea.HeightRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int Height { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Si prega di utilizzare la proprietà ChartArea.HeightRatioToChart, invece. Height = HeightRatioToChart * 4000. Questa proprietà sarà rimossa tra 12 mesi a partire da febbraio 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartAreaPropertyHeightDemo
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

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accedi all'area del grafico
            ChartArea chartArea = chart.ChartArea;

            // Dimostra la proprietà Height
            Console.WriteLine("Original Chart Area Height: " + chartArea.Height);
            
            // Modifica l'altezza
            chartArea.Height = 500;
            Console.WriteLine("Modified Chart Area Height: " + chartArea.Height);

            // Salva la cartella di lavoro
            workbook.Save("ChartAreaHeightDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


