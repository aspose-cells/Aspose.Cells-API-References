---
title: "Line.EndArrowLength"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Line. Specifica la lunghezza della punta della freccia per la fine di una linea"
type: docs
url: /it/net/aspose.cells.drawing/line/endarrowlength/
---
## Line.EndArrowLength property

Specifica la lunghezza della punta della freccia per la fine di una linea.

```csharp
public MsoArrowheadLength EndArrowLength { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Charts;
    using System;

    public class LinePropertyEndArrowLengthDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Crea un foglio di lavoro di esempio
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati per rendere l'esempio significativo
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["B1"].PutValue("Values");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["B3"].PutValue(40);

            try
            {
                // Aggiungi un grafico per dimostrare le proprietà della linea
                int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 15, 5);
                Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
                chart.NSeries.Add("A1:B3", true);

                // Ottieni le proprietà della linea dal bordo della serie del grafico
                Line line = chart.NSeries[0].Border;

                // Imposta un tipo di punta di freccia per dimostrare EndArrowLength
                line.EndType = MsoArrowheadStyle.Arrow;

                // Visualizza il valore corrente di EndArrowLength
                Console.WriteLine("Current EndArrowLength: " + line.EndArrowLength);

                // Imposta un nuovo valore per EndArrowLength
                line.EndArrowLength = MsoArrowheadLength.Long;
                Console.WriteLine("Updated EndArrowLength: " + line.EndArrowLength);

                // Salva la cartella di lavoro
                workbook.Save("EndArrowLengthDemo.xlsx");
                Console.WriteLine("EndArrowLength property demonstrated successfully.");
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


