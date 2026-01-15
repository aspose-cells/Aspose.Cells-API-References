---
title: Class ThreadedCommentAuthor
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.ThreadedCommentAuthor class. Represents the person who creates the threaded comments
type: docs
url: /net/aspose.cells/threadedcommentauthor/
---
## ThreadedCommentAuthor class

Represents the person who creates the threaded comments.

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
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassThreadedCommentAuthorDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a comment
            int commentIndex = worksheet.Comments.Add("C1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Initial comment";
            
            // Add threaded comment authors
            int authorIndex1 = workbook.Worksheets.ThreadedCommentAuthors.Add("Author1", "user1", "");
            ThreadedCommentAuthor author1 = workbook.Worksheets.ThreadedCommentAuthors[authorIndex1];
            
            // Add a threaded comment
            int threadedCommentIndex = comment.ThreadedComments.Add("Threaded comment text", author1);
            ThreadedComment threadedComment = comment.ThreadedComments[threadedCommentIndex];
            
            // Access and modify the author
            Console.WriteLine("Original author: " + threadedComment.Author.Name);
            threadedComment.Author.Name = "ModifiedAuthor";
            Console.WriteLine("Modified author: " + threadedComment.Author.Name);

            // Create a new author and assign it
            int authorIndex2 = workbook.Worksheets.ThreadedCommentAuthors.Add("Author2", "user2", "");
            ThreadedCommentAuthor author2 = workbook.Worksheets.ThreadedCommentAuthors[authorIndex2];
            threadedComment.Author = author2;
            Console.WriteLine("New author: " + threadedComment.Author.Name);
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


