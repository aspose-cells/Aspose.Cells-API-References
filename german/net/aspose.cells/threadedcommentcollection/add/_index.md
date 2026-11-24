---
title: "ThreadedCommentCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ThreadedCommentCollection-Methode. Fügt einen Threaded Comment hinzu"
type: docs
url: /de/net/aspose.cells/threadedcommentcollection/add/
---
## ThreadedCommentCollection.Add method

Fügt einen Threaded-Kommentar hinzu.

```csharp
public int Add(string text, ThreadedCommentAuthor author)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Text | String | Der Text des Threaded Comments. |
| Autor | ThreadedCommentAuthor | Der Autor des Threaded Comments |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentCollectionMethodAddWithStringThreadedCommentDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Daten für den Kontext hinzu
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Erstelle einen Threaded Comment-Autor mithilfe der ThreadedCommentAuthorCollection
                ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;
                int authorIndex = authors.Add("John Doe", "john.doe@example.com", "EXAMPLE_PROVIDER");
                ThreadedCommentAuthor author = authors[authorIndex];

                // Zugriff auf die Threaded Comments-Sammlung einer Zelle
                Comment comment = worksheet.Comments[worksheet.Comments.Add("A1")];
                ThreadedCommentCollection threadedComments = comment.ThreadedComments;

                // Rufen Sie die Add-Methode mit den Parametern String und ThreadedCommentAuthor auf
                int commentIndex = threadedComments.Add("This is a threaded comment", author);

                // Ergebnis anzeigen
                Console.WriteLine($"Added threaded comment at index: {commentIndex}");
                Console.WriteLine($"Comment text: {threadedComments[commentIndex].Notes}");
                Console.WriteLine($"Author: {threadedComments[commentIndex].Author.Name}");

                // Speichere die Arbeitsmappe
                workbook.Save("ThreadedCommentAddDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedCommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


