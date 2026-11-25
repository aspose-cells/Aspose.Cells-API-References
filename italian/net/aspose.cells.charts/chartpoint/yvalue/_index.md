---
title: "ChartPoint.YValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartPoint. Ottiene o imposta il valore Y del punto del grafico"
type: docs
url: /it/net/aspose.cells.charts/chartpoint/yvalue/
---
## ChartPoint.YValue property

Ottiene o imposta il valore Y del chart point.

```csharp
public object YValue { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPointPropertyYValueDemo
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
            worksheet.Cells["A5"].PutValue("D");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Aggiungi un grafico a colonne
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Ottieni i punti della prima serie
            Series series = chart.NSeries[0];
            var points = series.Points;

            // Dimostra la proprietà YValue
            Console.WriteLine("Y Values of Chart Points:");
            for (int i = 0; i < points.Count; i++)
            {
                Console.WriteLine($"Point {i + 1}: {points[i].YValue}");
            }

            // Modifica lo YValue di un punto
            points[2].YValue = 50;
            Console.WriteLine($"\nModified Point 3 YValue to: {points[2].YValue}");

            // Salva la cartella di lavoro
            workbook.Save("ChartPointYValueDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


