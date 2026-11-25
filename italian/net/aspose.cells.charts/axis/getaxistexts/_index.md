---
title: "Axis.GetAxisTexts"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Axis. Ottiene le etichette dell'asse dopo la chiamata al metodo Chart.Calculate"
type: docs
url: /it/net/aspose.cells.charts/axis/getaxistexts/
---
## Axis.GetAxisTexts method

Ottiene le etichette dell'asse dopo aver chiamato il metodo Chart.Calculate().

```csharp
public string[] GetAxisTexts()
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisMethodGetAxisTextsDemo
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
            worksheet.Cells["B2"].PutValue(8000);
            worksheet.Cells["B3"].PutValue(4000);
            worksheet.Cells["B4"].PutValue(-8000);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Calcola il grafico
            chart.Calculate();
            
            // Ottieni le etichette dell'asse
            string[] labels = chart.ValueAxis.GetAxisTexts();
            
            // Emetti le etichette
            Console.WriteLine("Value Axis Labels:");
            foreach (string label in labels)
            {
                Console.WriteLine(label);
            }
        }
    }
}
```

### Vedi anche

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


