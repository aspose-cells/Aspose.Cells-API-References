---
title: "ThreadedCommentAuthor.ProviderId"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ThreadedCommentAuthor. Ottiene l'ID del provider"
type: docs
url: /it/net/aspose.cells/threadedcommentauthor/providerid/
---
## ThreadedCommentAuthor.ProviderId property

Ottiene l'ID del provider.

```csharp
public string ProviderId { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentAuthorPropertyProviderIdDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Aggiungi un autore di commento a thread e ottieni il suo indice
                int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("John Doe", "JD123", "PROVIDER123");
                
                // Ottieni l'oggetto ThreadedCommentAuthor
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];
                
                // Visualizza il valore ProviderId (operazione di lettura)
                Console.WriteLine("Author ProviderId: " + author.ProviderId);
                
                // Crea un commento a thread utilizzando l'autore
                worksheet.Comments.AddThreadedComment("A1", "This is a sample comment", author);
                
                // Salva la cartella di lavoro
                workbook.Save("ThreadedCommentAuthorDemo.xlsx");
                
                Console.WriteLine("Demo completed successfully.");
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


