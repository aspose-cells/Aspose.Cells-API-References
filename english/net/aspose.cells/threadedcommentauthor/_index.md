---
title: Class ThreadedCommentAuthor
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.ThreadedCommentAuthor class. Represents the person who creates the threaded comments
type: docs
url: /net/aspose.cells/threadedcommentauthor/
---
## ThreadedCommentAuthor class

Represents the person who creates the threaded comments;

```csharp
public class ThreadedCommentAuthor
```

## Properties

| Name | Description |
| --- | --- |
| [Name](../../aspose.cells/threadedcommentauthor/name/) { get; set; } | Gets and sets the name. |
| [ProviderId](../../aspose.cells/threadedcommentauthor/providerid/) { get; set; } | Gets the id of the provider. |
| [UserId](../../aspose.cells/threadedcommentauthor/userid/) { get; set; } | Gets and sets the id of the user. |

### Examples

```csharp
// Called: ThreadedCommentAuthor author = threadedComment.Author;
[Test]
        public void Type_ThreadedCommentAuthor()
        {
           string testfile = Constants.sourcePath + (&quot;CellsNet49834.xlsx&quot;);

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
                            author.Name = &quot;James Bond&quot;;
                            author.UserId = &quot;JB&quot;;
                            threadedComment.Author = author;
                            Assert.AreEqual(&quot;James Bond&quot;,threadedComment.Author.Name);
                            Assert.AreEqual(&quot;JB&quot;, threadedComment.Author.UserId);
                        }
                    }
                    else
                    {
                        Console.WriteLine(comment.Author);
                        // try and change the author
                        comment.Author = &quot;James Bond&quot;;

                    }
                }
            }
            workbook.Save(Constants.destPath + &quot;CELLSNET49834.xlsx&quot;);
        }
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


