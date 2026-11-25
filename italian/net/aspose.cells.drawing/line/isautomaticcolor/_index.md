---
title: "Line.IsAutomaticColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Line. Indica se il colore della linea è assegnato automaticamente"
type: docs
url: /it/net/aspose.cells.drawing/line/isautomaticcolor/
---
## Line.IsAutomaticColor property

Indica se il colore della linea è assegnato automaticamente.

```csharp
public bool IsAutomaticColor { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class LinePropertyIsAutomaticColorDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per un chart
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            try
            {
                // Aggiungi un grafico a linee
                int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
                Chart chart = worksheet.Charts[chartIndex];
                chart.NSeries.Add("B2:B3", true);
                chart.NSeries.CategoryData = "A2:A3";

                // Accedi alla linea (bordo) della prima serie
                Line seriesLine = chart.NSeries[0].Border;

                // Leggi e visualizza il valore della proprietà IsAutomaticColor
                Console.WriteLine("IsAutomaticColor value: " + seriesLine.IsAutomaticColor);

                // Salva la cartella di lavoro
                workbook.Save("IsAutomaticColorDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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


