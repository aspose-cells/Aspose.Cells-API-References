---
title: ThreadedCommentCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: ThreadedCommentCollection method. Adds a threaded comment
type: docs
url: /net/aspose.cells/threadedcommentcollection/add/
---
## ThreadedCommentCollection.Add method

Adds a threaded comment;

```csharp
public int Add(string text, ThreadedCommentAuthor author)
```

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | The text of the threaded comment. |
| author | ThreadedCommentAuthor | The author of the threaded comment |

### Examples

```csharp
// Called: comment.ThreadedComments.Add(text, author);
private static void ThreadedCommentCollection_Method_Add(Worksheet worksheet, String cellName, String text, ThreadedCommentAuthor author)
        {
            Cell cell = worksheet.Cells[cellName];
            CommentCollection commentCollection = cell.Worksheet.Comments;
            Comment comment = commentCollection[cell.Row, cell.Column];
            if (comment == null)
            {
                int commentIdx = commentCollection.Add(cell.Row, cell.Column);
                comment = commentCollection[commentIdx];
            }
            comment.ThreadedComments.Add(text, author);
        }
```

### See Also

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedCommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


