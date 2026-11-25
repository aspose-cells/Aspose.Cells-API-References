---
title: "Enum MsoArrowheadLength"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Drawing.MsoArrowheadLength. Enumera la larghezza dell'estremità della linea del bordo della forma"
type: docs
url: /it/net/aspose.cells.drawing/msoarrowheadlength/
---
## MsoArrowheadLength enumeration

Enumera la larghezza dell'estremità della linea del bordo della forma.

```csharp
public enum MsoArrowheadLength
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Short | `0` | Lunghezza breve dell'estremità della linea |
| Medium | `1` | Lunghezza media dell'estremità della linea |
| Long | `2` | Lunghezza lunga dell'estremità della linea |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoArrowheadLengthDemo
    {
        public static void MsoArrowheadLengthExample()
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
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.SetChartDataRange("A1:B4", true);

            // Crea una forma di linea per il grafico
            Line line = chart.Line;

            // Imposta le lunghezze della punta della freccia
            line.BeginArrowLength = MsoArrowheadLength.Medium;
            line.EndArrowLength = MsoArrowheadLength.Long;

            // Restituisci le lunghezze delle punte di freccia
            Console.WriteLine("Begin Arrowhead Length: " + line.BeginArrowLength);
            Console.WriteLine("End Arrowhead Length: " + line.EndArrowLength);

            // Salva la cartella di lavoro
            workbook.Save("MsoArrowheadLengthExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


