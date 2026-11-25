---
title: "Enum MsoArrowheadWidth"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Drawing.MsoArrowheadWidth. Elenca la larghezza dell'estremità della linea del bordo della forma"
type: docs
url: /it/net/aspose.cells.drawing/msoarrowheadwidth/
---
## MsoArrowheadWidth enumeration

Enumera la larghezza dell'estremità della linea del bordo della forma.

```csharp
public enum MsoArrowheadWidth
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Narrow | `0` | Larghezza dell'estremità della linea corta. |
| Medium | `1` | Larghezza dell'estremità della linea media. |
| Wide | `2` | Larghezza dell'estremità della linea larga. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Charts;
    using System;

    public class MsoArrowheadWidthDemo
    {
        public static void MsoArrowheadWidthExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.SetChartDataRange("A1:B4", true);

            // Crea una forma di linea per il grafico
            Line line = chart.Line;

            // Imposta gli stili e le larghezze delle punte di freccia
            line.BeginType = MsoArrowheadStyle.Arrow;
            line.BeginArrowWidth = MsoArrowheadWidth.Wide;
            line.EndType = MsoArrowheadStyle.Arrow;
            line.EndArrowWidth = MsoArrowheadWidth.Narrow;

            // Restituisci gli stili e le larghezze delle punte di freccia
            Console.WriteLine("Begin Arrowhead Width: " + line.BeginArrowWidth);
            Console.WriteLine("End Arrowhead Width: " + line.EndArrowWidth);

            // Salva la cartella di lavoro
            workbook.Save("MsoArrowheadWidthExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


