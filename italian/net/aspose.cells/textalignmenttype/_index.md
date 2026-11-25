---
title: "Enum TextAlignmentType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.TextAlignmentType. Elenca i tipi di allineamento del testo"
type: docs
url: /it/net/aspose.cells/textalignmenttype/
---
## TextAlignmentType enumeration

Enumera i tipi di allineamento del testo.

```csharp
public enum TextAlignmentType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| General | `1792` | Rappresenta l'allineamento generale del testo. |
| Bottom | `528` | Rappresenta l'allineamento del testo in basso. |
| Center | `1802` | Rappresenta l'allineamento del testo al centro. |
| CenterAcross | `1286` | Rappresenta l'allineamento del testo centrato su tutta la larghezza. |
| Distributed | `807` | Rappresenta l'allineamento del testo distribuito. |
| Fill | `1284` | Rappresenta l'allineamento del testo riempito. |
| Justify | `1821` | Rappresenta l'allineamento del testo giustificato. |
| Left | `257` | Rappresenta l'allineamento del testo a sinistra. |
| Right | `259` | Rappresenta l'allineamento del testo a destra. |
| Top | `512` | Rappresenta l'allineamento del testo in alto. |
| JustifiedLow | `832` | Allinea il testo con una lunghezza di kashida regolata per il testo arabo. |
| ThaiDistributed | `896` | Distribuisce il testo tailandese in modo speciale, poiché ogni carattere è trattato come una parola. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TextAlignmentTypeDemo
    {
        public static void TextAlignmentTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Doe");

            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["B3"].PutValue(90);
            worksheet.Cells["B4"].PutValue(78);

            // Aggiungi un commento a una cella
            Comment comment = worksheet.Comments[worksheet.Comments.Add("A1")];
            comment.Note = "This is a comment.";
            comment.TextHorizontalAlignment = TextAlignmentType.Center;
            comment.TextVerticalAlignment = TextAlignmentType.Top;

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.SetChartDataRange("A1:B4", true);

            // Personalizza il titolo del grafico
            chart.Title.Text = "Scores Chart";
            chart.Title.TextHorizontalAlignment = TextAlignmentType.Center;
            chart.Title.TextVerticalAlignment = TextAlignmentType.Top;

            // Salva la cartella di lavoro
            workbook.Save("TextAlignmentTypeExample.xlsx");

            // Restituisci i risultati
            Console.WriteLine("Workbook saved successfully with text alignment settings.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


