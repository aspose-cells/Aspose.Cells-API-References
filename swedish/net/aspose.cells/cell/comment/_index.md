---
title: "Cell.Comment"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-egenskap. Hämtar kommentaren för denna cell"
type: docs
url: /sv/net/aspose.cells/cell/comment/
---
## Cell.Comment property

Hämtar kommentaren för den här cellen.

```csharp
public Comment Comment { get; }
```

### Anmärkningar

Om det inte finns någon kommentar som gäller för cellen, returneras null.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellPropertyCommentDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en kommentar till cell A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Cell");

            // Lägg till en kommentar till cellen
            Comment comment = cell.Comment;
            if (comment == null)
            {
                // Skapa en ny kommentar om ingen finns
                int commentIndex = worksheet.Comments.Add("A1");
                comment = worksheet.Comments[commentIndex];
                comment.Author = "Author Name";
                comment.Note = "This is a sample comment";
            }

            try
            {
                // Visa kommentarens egenskaper
                Console.WriteLine("Comment Author: " + comment.Author);
                Console.WriteLine("Comment Note: " + comment.Note);
                Console.WriteLine("Comment Row: " + comment.Row);
                Console.WriteLine("Comment Column: " + comment.Column);
                Console.WriteLine("Comment is Visible: " + comment.IsVisible);

                // Ändra några kommentar-egenskaper
                comment.Note = "Updated comment text";
                comment.IsVisible = true;

                // Visa uppdaterad kommentaranteckning
                Console.WriteLine("Updated Comment Note: " + comment.Note);

                // Spara arbetsboken
                workbook.Save("CommentDemo.xlsx");
                Console.WriteLine("Comment has been demonstrated and saved to CommentDemo.xlsx");
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

* class [Comment](../../comment/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


