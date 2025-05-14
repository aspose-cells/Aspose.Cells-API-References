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
// Called: int author1Index = workbook.Worksheets.ThreadedCommentAuthors.Add("Author 1", "author1", "OV");
public void ThreadedCommentAuthorCollection_Method_Add()
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

* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


