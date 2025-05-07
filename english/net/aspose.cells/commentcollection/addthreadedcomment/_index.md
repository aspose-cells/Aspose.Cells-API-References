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
// Called: comments.AddThreadedComment(2, 2, "This is a threaded comment.", author);
public static void Method_ThreadedCommentAuthor_()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Access the comments collection of the worksheet
            CommentCollection comments = worksheet.Comments;

            // Add a comment to cell A1
            int commentIndex1 = comments.Add(0, 0);
            Comment comment1 = comments[commentIndex1];
            comment1.Note = "First note.";
            comment1.Author = "Author1";
            comment1.Font.Name = "Times New Roman";

            // Add a comment to cell B2
            comments.Add("B2");
            Comment comment2 = comments["B2"];
            comment2.Note = "Second note.";
            comment2.Author = "Author2";

            // Add a threaded comment to cell C3
            int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("Author3", "user3", "provider3");
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];
            comments.AddThreadedComment(2, 2, "This is a threaded comment.", author);

            // Retrieve threaded comments from cell C3
            var threadedComments = comments.GetThreadedComments(2, 2);
            foreach (var threadedComment in threadedComments)
            {
                Console.WriteLine(threadedComment.Notes);
            }

            // Remove the comment at cell A1
            comments.RemoveAt(0, 0);

            // Clear all comments
            comments.Clear();

            // Save the workbook
            workbook.Save("CommentCollectionExample.xlsx");
            workbook.Save("CommentCollectionExample.pdf");
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
// Called: comments.AddThreadedComment("B3", "Test2", null);
[Test]
        public void Method_ThreadedCommentAuthor_()
        {
            Workbook workbook = new Workbook();
            CommentCollection comments = workbook.Worksheets[0].Comments;
            comments.AddThreadedComment("B3", "Test1", null);
            comments.AddThreadedComment("B3", "Test2", null);
            comments.AddThreadedComment("B3", "Test3", null);
            workbook.Save(Constants.destPath + "CELLSNET46656_001.xlsx");
        }
```

### See Also

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


