---
title: "Line.BeginArrowLength"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Line. Specifica la lunghezza della punta della freccia per l'inizio di una linea"
type: docs
url: /it/net/aspose.cells.drawing/line/beginarrowlength/
---
## Line.BeginArrowLength property

Specifica la lunghezza della punta della freccia per l'inizio di una linea.

```csharp
public MsoArrowheadLength BeginArrowLength { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class LinePropertyBeginArrowLengthDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Prepara dati semplici per un grafico
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

                // Imposta il BeginArrowLength su Long
                seriesLine.BeginArrowLength = MsoArrowheadLength.Long;

                // Leggi e visualizza il valore corrente di BeginArrowLength
                Console.WriteLine("BeginArrowLength value: " + seriesLine.BeginArrowLength);

                // Salva la cartella di lavoro (opzionale, solo per completare la demo)
                workbook.Save("BeginArrowLengthDemo.xlsx");
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

* enum [MsoArrowheadLength](../../msoarrowheadlength/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


