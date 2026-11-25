---
title: "Enum TextOrientationType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.TextOrientationType. Elenca i tipi di orientamento del testo"
type: docs
url: /it/net/aspose.cells/textorientationtype/
---
## TextOrientationType enumeration

Enumera i tipi di orientamento del testo.

```csharp
public enum TextOrientationType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| ClockWise | `0` | Ruota il testo di 90 gradi in senso orario. |
| CounterClockWise | `1` | Ruota il testo di 90 gradi in senso antiorario. |
| NoRotation | `2` | Rappresenta il valore predefinito. |
| TopToBottom | `3` | Visualizza il testo dall'alto verso il basso della cella. Testo impilato. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TextOrientationTypeDemo
    {
        public static void TextOrientationTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Hello, Aspose!");
            worksheet.Cells["A2"].PutValue("This is a test comment.");

            // Aggiungi un commento alla cella A1
            int commentIndex = worksheet.Comments.Add(0, 0);
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a comment with text orientation.";

            // Imposta diversi tipi di orientamento del testo per il commento
            comment.TextOrientationType = TextOrientationType.ClockWise;
            Console.WriteLine("Text Orientation: ClockWise");

            // Salva la cartella di lavoro
            workbook.Save("TextOrientationTypeExample_ClockWise.xlsx");

            // Cambia l'orientamento del testo in CounterClockWise
            comment.TextOrientationType = TextOrientationType.CounterClockWise;
            Console.WriteLine("Text Orientation: CounterClockWise");

            // Salva la cartella di lavoro
            workbook.Save("TextOrientationTypeExample_CounterClockWise.xlsx");

            // Cambia l'orientamento del testo in NoRotation
            comment.TextOrientationType = TextOrientationType.NoRotation;
            Console.WriteLine("Text Orientation: NoRotation");

            // Salva la cartella di lavoro
            workbook.Save("TextOrientationTypeExample_NoRotation.xlsx");

            // Cambia l'orientamento del testo in TopToBottom
            comment.TextOrientationType = TextOrientationType.TopToBottom;
            Console.WriteLine("Text Orientation: TopToBottom");

            // Salva la cartella di lavoro
            workbook.Save("TextOrientationTypeExample_TopToBottom.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


