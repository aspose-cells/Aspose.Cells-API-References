---
title: "Enum PlotEmptyCellsType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Charts.PlotEmptyCellsType enum. Rappresenta tutti i tipi di celle vuote di un grafico"
type: docs
url: /it/net/aspose.cells.charts/plotemptycellstype/
---
## PlotEmptyCellsType enumeration

Rappresenta tutti i tipi di celle vuote del tracciato di un grafico.

```csharp
public enum PlotEmptyCellsType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| NotPlotted | `0` | Non tracciato (lascia uno spazio) |
| Zero | `1` | Zero |
| Interpolated | `2` | Interpolato |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotEmptyCellsTypeDemo
    {
        public static void PlotEmptyCellsTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(null); // Empty cell
            worksheet.Cells["A5"].PutValue("D");
            worksheet.Cells["B5"].PutValue(40);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 7, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo di dati per il grafico
            chart.SetChartDataRange("A1:B5", true);

            // Imposta il titolo del grafico
            chart.Title.Text = "Plot Empty Cells Example";

            // Imposta come tracciare le celle vuote
            chart.PlotEmptyCellsType = PlotEmptyCellsType.Interpolated;

            // Salva la cartella di lavoro
            workbook.Save("PlotEmptyCellsTypeExample.xlsx");

            Console.WriteLine("Workbook saved successfully.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


