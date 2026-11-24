---
title: "ThreadedCommentAuthor.ProviderId"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ThreadedCommentAuthor-Eigenschaft. Liest die ID des Anbieters"
type: docs
url: /de/net/aspose.cells/threadedcommentauthor/providerid/
---
## ThreadedCommentAuthor.ProviderId property

Liest die ID des Anbieters.

```csharp
public string ProviderId { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentAuthorPropertyProviderIdDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Füge einen ThreadedCommentAuthor hinzu und erhalte dessen Index
                int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("John Doe", "JD123", "PROVIDER123");
                
                // Hole das ThreadedCommentAuthor-Objekt
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];
                
                // Zeige den ProviderId-Wert an (Lesevorgang)
                Console.WriteLine("Author ProviderId: " + author.ProviderId);
                
                // Erstelle einen ThreadedComment mit dem Autor
                worksheet.Comments.AddThreadedComment("A1", "This is a sample comment", author);
                
                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [ThreadedCommentAuthor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


