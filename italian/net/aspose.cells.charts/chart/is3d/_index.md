---
title: "Chart.Is3D"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Chart. Indica se il grafico è un grafico 3D"
type: docs
url: /it/net/aspose.cells.charts/chart/is3d/
---
## Chart.Is3D property

Indica se il grafico è un grafico 3D.

```csharp
public bool Is3D { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPropertyIs3DDemo
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
            worksheet.Cells["A5"].PutValue("Q4");

            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["B3"].PutValue(1500);
            worksheet.Cells["B4"].PutValue(1800);
            worksheet.Cells["B5"].PutValue(2100);

            // Aggiungi un grafico a colonne
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 6, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dei dati per il grafico
            chart.SetChartDataRange("A1:B5", true);

            // Visualizza il valore corrente di Is3D
            Console.WriteLine("Current Is3D value: " + chart.Is3D);

            // Crea una versione 3D del grafico
            int chart3DIndex = worksheet.Charts.Add(ChartType.Column3D, 6, 12, 20, 22);
            Chart chart3D = worksheet.Charts[chart3DIndex];
            chart3D.SetChartDataRange("A1:B5", true);

            // Visualizza il valore Is3D del grafico 3D
            Console.WriteLine("3D Chart Is3D value: " + chart3D.Is3D);

            // Salva la cartella di lavoro
            workbook.Save("ChartPropertyIs3DDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


