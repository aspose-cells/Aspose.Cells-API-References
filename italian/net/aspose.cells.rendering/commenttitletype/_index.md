---
title: "Enum CommentTitleType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Rendering.CommentTitleType. Rappresenta il tipo di titolo del commento durante il rendering quando il commento è impostato per essere visualizzato alla fine del foglio"
type: docs
url: /it/net/aspose.cells.rendering/commenttitletype/
---
## CommentTitleType enumeration

Rappresenta il tipo di titolo del commento durante il rendering quando il commento è impostato per essere visualizzato alla fine del foglio.

```csharp
public enum CommentTitleType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Cell | `0` | Rappresenta la cella del titolo del commento. |
| Comment | `1` | Rappresenta il commento del titolo del commento. |
| Note | `2` | Rappresenta la nota del titolo del commento. |
| Reply | `3` | Rappresenta la risposta del titolo del commento. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassCommentTitleTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Crea impostazioni di globalizzazione personalizzate
                SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

                // Dimostra tutti i valori dell'enum CommentTitleType
                Console.WriteLine("Available CommentTitleType values:");
                Console.WriteLine($"Cell: {(int)CommentTitleType.Cell}");
                Console.WriteLine($"Comment: {(int)CommentTitleType.Comment}");
                Console.WriteLine($"Note: {(int)CommentTitleType.Note}");
                Console.WriteLine($"Reply: {(int)CommentTitleType.Reply}");

                // Imposta titoli personalizzati per ogni tipo di commento
                globalizationSettings.SetCommentTitleName(CommentTitleType.Cell, "Custom Cell Title");
                globalizationSettings.SetCommentTitleName(CommentTitleType.Comment, "Custom Comment Title");
                globalizationSettings.SetCommentTitleName(CommentTitleType.Note, "Custom Note Title");
                globalizationSettings.SetCommentTitleName(CommentTitleType.Reply, "Custom Reply Title");

                // Applica le impostazioni di globalizzazione al workbook
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                // Aggiungi un commento per dimostrare la funzionalità
                int commentIndex = worksheet.Comments.Add("A1");
                Comment comment = worksheet.Comments[commentIndex];
                comment.Note = "This is a test comment";
                comment.Author = "Test Author";

                // Salva la cartella di lavoro
                workbook.Save("CommentTitleTypeDemo.xlsx");

                Console.WriteLine("CommentTitleType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in CommentTitleType demonstration: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


