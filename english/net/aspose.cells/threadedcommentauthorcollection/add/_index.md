---
title: ThreadedCommentAuthorCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: ThreadedCommentAuthorCollection method. Adds one thread comment person
type: docs
url: /net/aspose.cells/threadedcommentauthorcollection/add/
---
## ThreadedCommentAuthorCollection.Add method

Adds one thread comment person.

```csharp
public int Add(string name, string userId, string providerId)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the person. |
| userId | String |  |
| providerId | String | The id of the provider |

### Examples

```csharp
// Called: int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("Author3", "user3", "provider3");
public static void Method_String_()
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

* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


