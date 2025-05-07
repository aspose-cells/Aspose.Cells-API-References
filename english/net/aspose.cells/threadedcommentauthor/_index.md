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
// Called: ThreadedCommentAuthor author1 = workbook.Worksheets.ThreadedCommentAuthors[0];
[Test]
        public void Type_ThreadedCommentAuthor()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            int author1Index = workbook.Worksheets.ThreadedCommentAuthors.Add("Author 1", "author1", "OV");
            ThreadedCommentAuthor author1 = workbook.Worksheets.ThreadedCommentAuthors[0];
            FindOptions findOptions = new FindOptions();
            findOptions.RegexKey = true;
            findOptions.CaseSensitive = false;
            findOptions.SearchBackward = true;
            findOptions.LookInType = LookInType.Comments;
            addThreadedComment(worksheet, "C2", "1", author1);
            addThreadedComment(worksheet, "C2", "2", author1);
            addThreadedComment(worksheet, "C2", "3", author1);
            addThreadedComment(worksheet, "C2", "4", author1);
            Cell cell = worksheet.Cells.Find("4", null, findOptions);
            Assert.AreEqual(cell.Name,"C2");
            workbook.Save(Constants.destPath + "CellsNet47239.xlsx");
            workbook = new Workbook(Constants.destPath + "CellsNet47239.xlsx");
        }
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


