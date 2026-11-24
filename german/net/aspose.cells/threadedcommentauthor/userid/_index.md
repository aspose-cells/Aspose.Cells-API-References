---
title: "ThreadedCommentAuthor.UserId"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ThreadedCommentAuthor-Eigenschaft. Liest und schreibt die ID des Benutzers"
type: docs
url: /de/net/aspose.cells/threadedcommentauthor/userid/
---
## ThreadedCommentAuthor.UserId property

Liest und setzt die ID des Benutzers.

```csharp
public string UserId { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentAuthorPropertyUserIdDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Füge einen ThreadedCommentAuthor mit Name, userId und providerId hinzu
                int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("John Doe", "JD123", "PROVIDER123");

                // Hole das ThreadedCommentAuthor-Objekt
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];

                // Zeige den UserId-Wert an (Lesevorgang)
                Console.WriteLine("Author UserId: " + author.UserId);

                // Demonstriere das Setzen einer neuen UserId (Schreibvorgang)
                author.UserId = "NEW_USER_ID";
                Console.WriteLine("Updated UserId: " + author.UserId);

                // Erstelle einen ThreadedComment mit dem Autor
                worksheet.Comments.AddThreadedComment("A1", "This is a sample comment", author);

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [ThreadedCommentAuthor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


