---
title: "Axis.MajorUnit"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Axis. Rappresenta le unità principali per l'asse"
type: docs
url: /it/net/aspose.cells.charts/axis/majorunit/
---
## Axis.MajorUnit property

Rappresenta le unità principali per l'asse.

```csharp
public double MajorUnit { get; set; }
```

### Osservazioni

Le unità principali devono essere maggiori di zero.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMajorUnitDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Cat " + i);
                worksheet.Cells["B" + (i + 1)].PutValue(i * 10);
            }

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B11", true);
            chart.NSeries.CategoryData = "A2:A11";

            // Ottieni l'asse delle categorie
            Axis axis = chart.CategoryAxis;

            // Visualizza l'unità principale iniziale
            Console.WriteLine("Initial Major Unit: " + axis.MajorUnit);

            // Imposta una nuova unità principale
            axis.MajorUnit = 3;
            Console.WriteLine("Modified Major Unit: " + axis.MajorUnit);

            // Salva la cartella di lavoro
            workbook.Save("AxisMajorUnitDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


