---
title: "ThreadedCommentCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ThreadedCommentCollection. Aggiunge un commento a thread"
type: docs
url: /it/net/aspose.cells/threadedcommentcollection/add/
---
## ThreadedCommentCollection.Add method

Aggiunge un commento a thread.

```csharp
public int Add(string text, ThreadedCommentAuthor author)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| testo | String | Il testo del commento a thread. |
| autore | ThreadedCommentAuthor | L'autore del commento a thread |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentCollectionMethodAddWithStringThreadedCommentDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati per il contesto
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Crea un autore di commenti a thread utilizzando ThreadedCommentAuthorCollection
                ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;
                int authorIndex = authors.Add("John Doe", "john.doe@example.com", "EXAMPLE_PROVIDER");
                ThreadedCommentAuthor author = authors[authorIndex];

                // Accedi alla raccolta di commenti a thread di una cella
                Comment comment = worksheet.Comments[worksheet.Comments.Add("A1")];
                ThreadedCommentCollection threadedComments = comment.ThreadedComments;

                // Chiama il metodo Add con parametri String e ThreadedCommentAuthor
                int commentIndex = threadedComments.Add("This is a threaded comment", author);

                // Visualizza il risultato
                Console.WriteLine($"Added threaded comment at index: {commentIndex}");
                Console.WriteLine($"Comment text: {threadedComments[commentIndex].Notes}");
                Console.WriteLine($"Author: {threadedComments[commentIndex].Author.Name}");

                // Salva la cartella di lavoro
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

### Vedi anche

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedCommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


