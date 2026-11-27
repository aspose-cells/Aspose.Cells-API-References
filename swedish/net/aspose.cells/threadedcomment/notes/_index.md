---
title: "ThreadedComment.Notes"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThreadedComment-egenskap. Hämtar och anger texten för kommentaren"
type: docs
url: /sv/net/aspose.cells/threadedcomment/notes/
---
## ThreadedComment.Notes property

Hämtar och anger texten för kommentaren.

```csharp
public string Notes { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentPropertyNotesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Skapa eller hämta en författare för trådad kommentar
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors["User1"];
                author.Name = "User1";

                // Lägg till en trådad kommentar till cell A1 (rad 0, kolumn 0) med initial text
                worksheet.Comments.AddThreadedComment(0, 0, "Initial comment text", author);

                // Hämta den nyligen tillagda trådade kommentaren
                ThreadedComment threadedComment = worksheet.Comments[0].ThreadedComments[0];

                // Uppdatera Notes-egenskapen (kommentartexten)
                threadedComment.Notes = "Updated comment notes";

                // Läs och visa värdet för Notes-egenskapen
                Console.WriteLine("Threaded comment Notes: " + threadedComment.Notes);

                // Spara arbetsboken (valfritt)
                workbook.Save("ThreadedCommentNotesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [ThreadedComment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


