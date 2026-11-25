---
title: "Chart.Elevation"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà del grafico. Rappresenta l'elevazione della vista del grafico 3D in gradi"
type: docs
url: /it/net/aspose.cells.charts/chart/elevation/
---
## Chart.Elevation property

Rappresenta l'elevazione della visualizzazione del grafico 3-D, in gradi.

```csharp
public int Elevation { get; set; }
```

### Osservazioni

L'elevazione del grafico è l'altezza a cui visualizzi il grafico, in gradi. Il valore predefinito è 15 per la maggior parte dei tipi di grafico. Il valore di questa proprietà deve essere compreso tra -90 e 90, eccetto per i grafici a barre 3-D, dove deve essere compreso tra 0 e 44.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyElevationDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Aggiungi un grafico a colonne 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Imposta la proprietà elevation (angolo in gradi)
            chart.Elevation = 30;
            
            // Salva la cartella di lavoro
            workbook.Save("ChartElevationDemo.xlsx");

            Console.WriteLine("Chart created with elevation set to 30 degrees.");
        }
    }
}
```

### Vedi anche

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


