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
// Called: Assert.AreEqual(&amp;quot;JB&amp;quot;, threadedComment.Author.UserId);
[Test]
        public void Property_UserId()
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

* class [ThreadedCommentAuthor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


