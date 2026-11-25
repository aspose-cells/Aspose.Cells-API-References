---
title: "Axis.LogBase"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà dell'asse. Rappresenta la base logaritmica. Il valore predefinito è 10"
type: docs
url: /it/net/aspose.cells.charts/axis/logbase/
---
## Axis.LogBase property

Rappresenta la base logaritmica. Il valore predefinito è 10.

```csharp
public double LogBase { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyLogBaseDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("X Values");
            worksheet.Cells["B1"].PutValue("Y Values");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells[$"A{i}"].PutValue(Math.Pow(2, i-2)); // Exponential values
                worksheet.Cells[$"B{i}"].PutValue(i * 10);
            }

            // Crea un grafico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Aggiungi serie
            chart.NSeries.Add($"B2:B10", true);
            chart.NSeries[0].XValues = $"A2:A10";
            chart.NSeries[0].Name = "Logarithmic Series";

            // Configura l'asse logaritmico
            chart.CategoryAxis.IsLogarithmic = true;
            chart.CategoryAxis.LogBase = 2; // Set logarithmic base to 2
            chart.CategoryAxis.Title.Text = "Logarithmic Scale (Base 2)";
            
            // Salva la cartella di lavoro
            workbook.Save("AxisPropertyLogBaseDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


