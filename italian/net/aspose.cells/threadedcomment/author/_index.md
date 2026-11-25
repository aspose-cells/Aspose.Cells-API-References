---
title: "ThreadedComment.Author"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ThreadedComment. Ottiene l'autore del commento"
type: docs
url: /it/net/aspose.cells/threadedcomment/author/
---
## ThreadedComment.Author property

Ottiene l'autore del commento.

```csharp
public ThreadedCommentAuthor Author { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentPropertyAuthorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Ottieni l'autore predefinito del commento a thread dal workbook
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[0];
                author.Name = "John Doe";
                author.UserId = "john.doe@example.com";

                // Aggiungi un commento a thread alla cella A1 (riga 0, colonna 0)
                worksheet.Comments.AddThreadedComment(0, 0, "Sample comment", author);

                // Ottieni il primo commento a thread
                ThreadedComment comment = worksheet.Comments[0].ThreadedComments[0];

                // Visualizza il valore della proprietà Author (operazione di lettura)
                Console.WriteLine("Author Name: " + comment.Author.Name);
                Console.WriteLine("Author UserId: " + comment.Author.UserId);
                Console.WriteLine("Author ProviderId: " + comment.Author.ProviderId);

                // Dimostra l'impostazione della proprietà Author (poiché è lettura/scrittura)
                ThreadedCommentAuthor newAuthor = workbook.Worksheets.ThreadedCommentAuthors[0];
                newAuthor.Name = "Jane Smith";
                newAuthor.UserId = "jane.smith@example.com";
                comment.Author = newAuthor;

                // Visualizza il valore aggiornato della proprietà Author
                Console.WriteLine("Updated Author Name: " + comment.Author.Name);
                Console.WriteLine("Updated Author UserId: " + comment.Author.UserId);

                // Salva la cartella di lavoro
                workbook.Save("ThreadedCommentAuthorDemo.xlsx");
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
* class [ThreadedComment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


