---
title: "ThreadedCommentAuthor.UserId"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ThreadedCommentAuthor. Ottiene e imposta l'ID dell'utente"
type: docs
url: /it/net/aspose.cells/threadedcommentauthor/userid/
---
## ThreadedCommentAuthor.UserId property

Ottiene e imposta l'ID dell'utente.

```csharp
public string UserId { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentAuthorPropertyUserIdDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Aggiungi un autore di commento a thread con nome, userId e providerId
                int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("John Doe", "JD123", "PROVIDER123");

                // Ottieni l'oggetto ThreadedCommentAuthor
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];

                // Visualizza il valore UserId (operazione di lettura)
                Console.WriteLine("Author UserId: " + author.UserId);

                // Dimostra l'impostazione di un nuovo UserId (operazione di scrittura)
                author.UserId = "NEW_USER_ID";
                Console.WriteLine("Updated UserId: " + author.UserId);

                // Crea un commento a thread utilizzando l'autore
                worksheet.Comments.AddThreadedComment("A1", "This is a sample comment", author);

                // Salva la cartella di lavoro
                workbook.Save("UserIdDemo.xlsx");

                Console.WriteLine("UserId property demonstration completed successfully.");
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

* class [ThreadedCommentAuthor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


