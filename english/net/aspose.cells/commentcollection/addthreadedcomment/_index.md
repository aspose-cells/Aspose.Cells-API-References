---
title: CommentCollection.AddThreadedComment
second_title: Aspose.Cells for .NET API Reference
description: CommentCollection method. Adds a threaded comment
type: docs
url: /net/aspose.cells/commentcollection/addthreadedcomment/
---
## AddThreadedComment(int, int, string, ThreadedCommentAuthor) {#addthreadedcomment}

Adds a threaded comment.

```csharp
public int AddThreadedComment(int row, int column, string text, ThreadedCommentAuthor author)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Cell row index. |
| column | Int32 | Cell column index. |
| text | String | The text of the comment |
| author | ThreadedCommentAuthor | The user of this threaded comment. |

### Return Value

[`ThreadedComment`](../../threadedcomment/) object index.

### Examples

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

### See Also

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddThreadedComment(string, string, ThreadedCommentAuthor) {#addthreadedcomment_1}

Adds a threaded comment.

```csharp
public int AddThreadedComment(string cellName, string text, ThreadedCommentAuthor author)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | The name of the cell. |
| text | String | The text of the comment |
| author | ThreadedCommentAuthor | The user of this threaded comment. |

### Return Value

[`ThreadedComment`](../../threadedcomment/) object index.

### Examples

```csharp
// Called: comments.AddThreadedComment("B3", "Test1", null);
public void CommentCollection_Method_AddThreadedComment()
{
    Workbook workbook = new Workbook();
    CommentCollection comments = workbook.Worksheets[0].Comments;
    comments.AddThreadedComment("B3", "Test1", null);
    comments.AddThreadedComment("B3", "Test2", null);
    comments.AddThreadedComment("B3", "Test3", null);
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


