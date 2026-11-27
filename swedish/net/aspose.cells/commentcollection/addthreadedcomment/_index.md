---
title: "CommentCollection.AddThreadedComment"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CommentCollection-metoden. Lägger till en trådad kommentar"
type: docs
url: /sv/net/aspose.cells/commentcollection/addthreadedcomment/
---
## AddThreadedComment(int, int, string, ThreadedCommentAuthor) {#addthreadedcomment}

Lägger till en trådad kommentar.

```csharp
public int AddThreadedComment(int row, int column, string text, ThreadedCommentAuthor author)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Cellradindex. |
| column | Int32 | Cellkolumnindex. |
| text | String | Texten i kommentaren |
| författare | ThreadedCommentAuthor | Användaren av denna trådade kommentar. |

### Returvärde

[`ThreadedComment`](../../threadedcomment/) object index.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionMethodAddThreadedCommentWithInt32Int32StringThreadedCommenDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            CommentCollection comments = worksheet.Comments;
            
            int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("Demo Author", "demoUser", "testProvider");
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];
            
            comments.AddThreadedComment(1, 1, "This is a threaded comment demo.", author);
            
            var threadedComments = comments.GetThreadedComments(1, 1);
            foreach (var comment in threadedComments)
            {
                Console.WriteLine(comment.Notes);
            }

            workbook.Save("ThreadedCommentDemo.xlsx");
        }
    }
}
```

### Se även

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddThreadedComment(string, string, ThreadedCommentAuthor) {#addthreadedcomment_1}

Lägger till en trådad kommentar.

```csharp
public int AddThreadedComment(string cellName, string text, ThreadedCommentAuthor author)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellName | String | Namnet på cellen. |
| text | String | Texten i kommentaren |
| författare | ThreadedCommentAuthor | Användaren av denna trådade kommentar. |

### Returvärde

[`ThreadedComment`](../../threadedcomment/) object index.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionMethodAddThreadedCommentWithStringStringThreadedCommentDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("John Doe", "JD", "");
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];
            
            CommentCollection comments = worksheet.Comments;
            comments.AddThreadedComment("B3", "Initial comment text", author);
            comments.AddThreadedComment("C5", "Follow-up comment", author);
            
            workbook.Save("ThreadedCommentsOutput.xlsx");
        }
    }
}
```

### Se även

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


