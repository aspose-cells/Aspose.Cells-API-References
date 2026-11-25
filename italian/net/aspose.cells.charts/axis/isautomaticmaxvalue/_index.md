---
title: "Axis.IsAutomaticMaxValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Axis. Indica se il valore massimo è assegnato automaticamente"
type: docs
url: /it/net/aspose.cells.charts/axis/isautomaticmaxvalue/
---
## Axis.IsAutomaticMaxValue property

Indica se il valore massimo è assegnato automaticamente.

```csharp
public bool IsAutomaticMaxValue { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsAutomaticMaxValueDemo
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
            
            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ottieni l'asse dei valori
            Axis valueAxis = chart.ValueAxis;

            // Dimostra la proprietà IsAutomaticMaxValue
            Console.WriteLine("Initial IsAutomaticMaxValue: " + valueAxis.IsAutomaticMaxValue);
            Console.WriteLine("Initial MaxValue: " + valueAxis.MaxValue);

            // Disabilita il valore massimo automatico e imposta un valore personalizzato
            valueAxis.IsAutomaticMaxValue = false;
            valueAxis.MaxValue = 40;
            Console.WriteLine("After change - IsAutomaticMaxValue: " + valueAxis.IsAutomaticMaxValue);
            Console.WriteLine("After change - MaxValue: " + valueAxis.MaxValue);

            // Riattiva il valore massimo automatico
            valueAxis.IsAutomaticMaxValue = true;
            Console.WriteLine("After re-enabling - IsAutomaticMaxValue: " + valueAxis.IsAutomaticMaxValue);
            Console.WriteLine("After re-enabling - MaxValue: " + valueAxis.MaxValue);

            // Salva la cartella di lavoro
            workbook.Save("AxisPropertyIsAutomaticMaxValueDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


