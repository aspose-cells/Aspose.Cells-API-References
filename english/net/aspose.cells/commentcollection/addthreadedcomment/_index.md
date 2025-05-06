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
// Called: comments.AddThreadedComment(2, 2, &amp;quot;This is a threaded comment.&amp;quot;, author);
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
            comment1.Note = &quot;First note.&quot;;
            comment1.Author = &quot;Author1&quot;;
            comment1.Font.Name = &quot;Times New Roman&quot;;

            // Add a comment to cell B2
            comments.Add(&quot;B2&quot;);
            Comment comment2 = comments[&quot;B2&quot;];
            comment2.Note = &quot;Second note.&quot;;
            comment2.Author = &quot;Author2&quot;;

            // Add a threaded comment to cell C3
            int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add(&quot;Author3&quot;, &quot;user3&quot;, &quot;provider3&quot;);
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];
            comments.AddThreadedComment(2, 2, &quot;This is a threaded comment.&quot;, author);

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
            workbook.Save(&quot;CommentCollectionExample.xlsx&quot;);
            workbook.Save(&quot;CommentCollectionExample.pdf&quot;);
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
// Called: comments.AddThreadedComment(&amp;quot;B3&amp;quot;, &amp;quot;Test1&amp;quot;, null);
[Test]
        public void Method_ThreadedCommentAuthor_()
        {
            Workbook workbook = new Workbook();
            CommentCollection comments = workbook.Worksheets[0].Comments;
            comments.AddThreadedComment(&quot;B3&quot;, &quot;Test1&quot;, null);
            comments.AddThreadedComment(&quot;B3&quot;, &quot;Test2&quot;, null);
            comments.AddThreadedComment(&quot;B3&quot;, &quot;Test3&quot;, null);
            workbook.Save(Constants.destPath + &quot;CELLSNET46656_001.xlsx&quot;);
        }
```

### See Also

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


