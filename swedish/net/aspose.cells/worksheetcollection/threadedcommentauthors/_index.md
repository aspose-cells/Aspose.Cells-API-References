---
title: "WorksheetCollection.ThreadedCommentAuthors"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorksheetCollection-egenskap. Hämtar listan över trådade kommentarsförfattare"
type: docs
url: /sv/net/aspose.cells/worksheetcollection/threadedcommentauthors/
---
## WorksheetCollection.ThreadedCommentAuthors property

Hämtar listan över författare till trådade kommentarer.

```csharp
public ThreadedCommentAuthorCollection ThreadedCommentAuthors { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyThreadedCommentAuthorsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en trådad kommentarsförfattare
            int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("Demo Author", "demo", "DA");

            // Hämta författaren vi just lade till
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];

            // Lägg till trådade kommentarer till cell C2
            AddThreadedComment(worksheet, "C2", "First comment", author);
            AddThreadedComment(worksheet, "C2", "Second comment", author);
            AddThreadedComment(worksheet, "C2", "Third comment", author);

            // Spara arbetsboken
            workbook.Save("ThreadedCommentsDemo.xlsx");
        }

        private static void AddThreadedComment(Worksheet worksheet, string cellName, string text, ThreadedCommentAuthor author)
        {
            // Hämta cellen där vi vill lägga till kommentaren
            Cell cell = worksheet.Cells[cellName];
            
            // Lägg till en trådad kommentar (returnerar void, inte ThreadedComment)
            worksheet.Comments.AddThreadedComment(cellName, text, author);
        }
    }
}
```

### Se även

* class [ThreadedCommentAuthorCollection](../../threadedcommentauthorcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


