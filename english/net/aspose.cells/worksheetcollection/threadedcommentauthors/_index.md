---
title: WorksheetCollection.ThreadedCommentAuthors
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection property. Gets the list of threaded comment authors
type: docs
url: /net/aspose.cells/worksheetcollection/threadedcommentauthors/
---
## WorksheetCollection.ThreadedCommentAuthors property

Gets the list of threaded comment authors.

```csharp
public ThreadedCommentAuthorCollection ThreadedCommentAuthors { get; }
```

### Examples

```csharp
// Called: int author1Index = workbook.Worksheets.ThreadedCommentAuthors.Add("Author 1", "author1", "OV");
public void WorksheetCollection_Property_ThreadedCommentAuthors()
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
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [ThreadedCommentAuthorCollection](../../threadedcommentauthorcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


