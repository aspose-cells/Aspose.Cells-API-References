---
title: "CommentCollection.GetThreadedComments"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CommentCollection-metod. Hämtar de trådade kommentarerna efter rad- och kolumnindex"
type: docs
url: /sv/net/aspose.cells/commentcollection/getthreadedcomments/
---
## GetThreadedComments(int, int) {#getthreadedcomments}

Hämtar de trådade kommentarerna efter rad- och kolumnindex.

```csharp
public ThreadedCommentCollection GetThreadedComments(int row, int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindexet. |
| column | Int32 | Kolumnindexet. |

### Exempel

```csharp

[C#]
ThreadedCommentCollection threadedComments1 = comments.GetThreadedComments(1, 1);
for (int i = 0; i < threadedComments1.Count; ++i)
{
    ThreadedComment tc = threadedComments1[i];
    string note = tc.Notes;
}
```

### Se även

* class [ThreadedCommentCollection](../../threadedcommentcollection/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetThreadedComments(string) {#getthreadedcomments_1}

Hämtar de trådade kommentarerna efter cellnamn.

```csharp
public ThreadedCommentCollection GetThreadedComments(string cellName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellName | String | Namnet på cellen. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionMethodGetThreadedCommentsWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en trådad kommentar-författare och hämta författaren efter index
            int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("John Doe", "JD", "1");
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];

            // Lägg till en trådad kommentar i cell B2
            worksheet.Comments.AddThreadedComment("B2", "Initial comment", author);

            // Hämta alla trådade kommentarer för cell B2
            ThreadedCommentCollection threadedComments = worksheet.Comments.GetThreadedComments("B2");

            // Visa de trådade kommentarerna
            foreach (ThreadedComment comment in threadedComments)
            {
                Console.WriteLine($"Comment by {comment.Author.Name}: {comment.Notes}");
            }
        }
    }
}
```

### Se även

* class [ThreadedCommentCollection](../../threadedcommentcollection/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


