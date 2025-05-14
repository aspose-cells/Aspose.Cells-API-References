---
title: ThreadedCommentAuthor.UserId
second_title: Aspose.Cells for .NET API Reference
description: ThreadedCommentAuthor property. Gets and sets the id of the user
type: docs
url: /net/aspose.cells/threadedcommentauthor/userid/
---
## ThreadedCommentAuthor.UserId property

Gets and sets the id of the user.

```csharp
public string UserId { get; set; }
```

### Examples

```csharp
// Called: author.UserId = "JB";
public void ThreadedCommentAuthor_Property_UserId()
{
   string testfile = Constants.sourcePath + ("example.xlsx");

    var workbook = new Aspose.Cells.Workbook(testfile);

    foreach (Worksheet worksheet in workbook.Worksheets)
    {
        foreach (Comment comment in worksheet.Comments)
        {
            if (comment.IsThreadedComment)
            {
                foreach (ThreadedComment threadedComment in comment.ThreadedComments)
                {
                    Console.WriteLine(threadedComment.Author.Name);
                    Console.WriteLine(threadedComment.Author.UserId);

                    // try and change the author
                    ThreadedCommentAuthor author = threadedComment.Author;
                    author.Name = "James Bond";
                    author.UserId = "JB";
                    threadedComment.Author = author;
                    Assert.AreEqual("James Bond",threadedComment.Author.Name);
                    Assert.AreEqual("JB", threadedComment.Author.UserId);
                }
            }
            else
            {
                Console.WriteLine(comment.Author);
                // try and change the author
                comment.Author = "James Bond";

            }
        }
    }
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [ThreadedCommentAuthor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


