---
title: "Axis.IsAutomaticMinorUnit"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà dell'asse. Indica se l'unità minore dell'asse è assegnata automaticamente"
type: docs
url: /it/net/aspose.cells.charts/axis/isautomaticminorunit/
---
## Axis.IsAutomaticMinorUnit property

Indica se l'unità secondaria dell'asse è assegnata automaticamente.

```csharp
public bool IsAutomaticMinorUnit { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsAutomaticMinorUnitDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Ottieni l'asse dei valori
            Axis valueAxis = chart.ValueAxis;

            // Dimostra la proprietà IsAutomaticMinorUnit
            Console.WriteLine("Initial IsAutomaticMinorUnit: " + valueAxis.IsAutomaticMinorUnit);
            
            // Imposta l'unità minore manualmente
            valueAxis.IsAutomaticMinorUnit = false;
            valueAxis.MinorUnit = 2;
            Console.WriteLine("After setting manually - IsAutomaticMinorUnit: " + valueAxis.IsAutomaticMinorUnit);
            Console.WriteLine("MinorUnit: " + valueAxis.MinorUnit);

            // Ripristina su automatico
            valueAxis.IsAutomaticMinorUnit = true;
            Console.WriteLine("After setting automatic - IsAutomaticMinorUnit: " + valueAxis.IsAutomaticMinorUnit);

            // Salva la cartella di lavoro
            workbook.Save("AxisPropertyIsAutomaticMinorUnitDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


