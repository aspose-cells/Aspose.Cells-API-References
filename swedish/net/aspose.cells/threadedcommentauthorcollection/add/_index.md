---
title: "ThreadedCommentAuthorCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThreadedCommentAuthorCollection-metod. Lägger till en trådkommentarperson"
type: docs
url: /sv/net/aspose.cells/threadedcommentauthorcollection/add/
---
## ThreadedCommentAuthorCollection.Add method

Lägger till en trådkommentarperson.

```csharp
public int Add(string name, string userId, string providerId)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | String | Namnet på personen. |
| userId | String |  |
| providerId | String | Leverantörens ID |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentAuthorCollectionMethodAddWithStringStringStringDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en trådad kommentarsförfattare
            int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("Test Author", "testuser", "TA");

            // Hämta den tillagda författaren
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];

            // Lägg till trådade kommentarer med författaren
            worksheet.Comments.AddThreadedComment("C2", "First comment", author);
            worksheet.Comments.AddThreadedComment("C2", "Second comment", author);

            // Spara arbetsboken
            workbook.Save("ThreadedCommentsExample.xlsx");
        }
    }
}
```

### Se även

* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


