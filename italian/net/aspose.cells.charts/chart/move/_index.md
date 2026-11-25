---
title: "Chart.Move"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Chart. Sposta il grafico in una posizione specificata"
type: docs
url: /it/net/aspose.cells.charts/chart/move/
---
## Chart.Move method

Sposta il grafico in una posizione specificata.

```csharp
public void Move(int topRow, int leftColumn, int bottomRow, int rightColumn)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| leftColumn | Int32 | Indice della colonna in alto a sinistra. |
| topRow | Int32 | Indice della riga in alto a sinistra. |
| rightColumn | Int32 | Indice della colonna in basso a destra |
| bottomRow | Int32 | Indice della riga in basso a destra |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartMethodMoveWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Posizione originale del grafico
                Console.WriteLine($"Original position - topRow: {chart.ChartObject.UpperLeftRow}, leftColumn: {chart.ChartObject.UpperLeftColumn}");

                // Sposta il grafico nella nuova posizione (righe 10-20, colonne 2-8)
                chart.Move(10, 2, 20, 8);

                // Visualizza la nuova posizione
                Console.WriteLine($"New position - topRow: {chart.ChartObject.UpperLeftRow}, leftColumn: {chart.ChartObject.UpperLeftColumn}");

                // Salva la cartella di lavoro
                workbook.Save("ChartMoveDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Move method: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


