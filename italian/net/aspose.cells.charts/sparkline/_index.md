---
title: "Classe Sparkline"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Charts.Sparkline classe. Uno sparkline rappresenta un piccolo grafico o immagine in una cella del foglio di lavoro che fornisce una rappresentazione visiva dei dati"
type: docs
url: /it/net/aspose.cells.charts/sparkline/
---
## Sparkline class

Una sparkline rappresenta un piccolo grafico o immagine in una cella del foglio di lavoro che fornisce una rappresentazione visiva dei dati.

```csharp
public class Sparkline
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Column](../../aspose.cells.charts/sparkline/column/) { get; } | Ottiene l'indice di colonna dello sparkline. |
| [DataRange](../../aspose.cells.charts/sparkline/datarange/) { get; set; } | Rappresenta l'intervallo di dati dello sparkline. |
| [Row](../../aspose.cells.charts/sparkline/row/) { get; } | Ottiene l'indice di riga dello sparkline. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [ToImage](../../aspose.cells.charts/sparkline/toimage/#toimage)(ImageOrPrintOptions) | Converte uno sparkline in un'immagine. |
| [ToImage](../../aspose.cells.charts/sparkline/toimage/#toimage_1)(Stream, ImageOrPrintOptions) | Converte uno sparkline in un'immagine. |
| [ToImage](../../aspose.cells.charts/sparkline/toimage/#toimage_2)(string, ImageOrPrintOptions) | Converte uno sparkline in un'immagine. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SparklineDemo
    {
        public static void SparklineExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati al worksheet
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Definisci il CellArea per lo sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Aggiungi un gruppo di sparkline al foglio di lavoro
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, sheet.Name + "!A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Aggiungi uno sparkline al gruppo
            idx = group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 5);
            Sparkline line = group.Sparklines[idx];

            // Dettagli dello sparkline
            Console.WriteLine("Sparkline data range: " + line.DataRange + ", row: " + line.Row + ", column: " + line.Column);

            // Salva lo sparkline come immagine
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = Aspose.Cells.Drawing.ImageType.Png,
                HorizontalResolution = 300,
                VerticalResolution = 300
            };
            line.ToImage("output.png", options);

            // Salva la cartella di lavoro
            workbook.Save("SparklineExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


