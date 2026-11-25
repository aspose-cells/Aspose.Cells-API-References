---
title: "Line.IsAuto"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Line. Indica se questo stile di linea è assegnato automaticamente"
type: docs
url: /it/net/aspose.cells.drawing/line/isauto/
---
## Line.IsAuto property

Indica se questo stile di linea è assegnato automaticamente.

```csharp
public bool IsAuto { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Charts;
    using System;

    public class LinePropertyIsAutoDemo
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
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            try
            {
                // Aggiungi un grafico a linee
                int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
                Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

                // Imposta l'intervallo dati del grafico
                chart.NSeries.Add("B2:B3", true);
                chart.NSeries.CategoryData = "A2:A3";

                // Accedi alle proprietà della linea della serie
                Aspose.Cells.Charts.Series series = chart.NSeries[0];
                Line line = series.Border;

                // Visualizza il valore corrente di IsAuto
                Console.WriteLine("Initial IsAuto value: " + line.IsAuto);

                // Imposta IsAuto su true
                line.IsAuto = true;
                Console.WriteLine("After setting to true, IsAuto value: " + line.IsAuto);

                // Imposta IsAuto su false
                line.IsAuto = false;
                Console.WriteLine("After setting to false, IsAuto value: " + line.IsAuto);

                // Salva la cartella di lavoro
                workbook.Save("IsAutoDemo.xlsx");
                Console.WriteLine("IsAuto property has been demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


