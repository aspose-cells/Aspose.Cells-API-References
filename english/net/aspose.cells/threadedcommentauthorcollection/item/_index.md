---
title: ThreadedCommentAuthorCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ThreadedCommentAuthorCollection property. Gets the person who create threaded comments
type: docs
url: /net/aspose.cells/threadedcommentauthorcollection/item/
---
## ThreadedCommentAuthorCollection indexer (1 of 2)

Gets the person who create threaded comments.

```csharp
public ThreadedCommentAuthor this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index |

### Examples

```csharp
// Called: ThreadedCommentAuthor author1 = workbook.Worksheets.ThreadedCommentAuthors[0];
[Test]
        public void Property_Int32_()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            int author1Index = workbook.Worksheets.ThreadedCommentAuthors.Add(&quot;Author 1&quot;, &quot;author1&quot;, &quot;OV&quot;);
            ThreadedCommentAuthor author1 = workbook.Worksheets.ThreadedCommentAuthors[0];
            FindOptions findOptions = new FindOptions();
            findOptions.RegexKey = true;
            findOptions.CaseSensitive = false;
            findOptions.SearchBackward = true;
            findOptions.LookInType = LookInType.Comments;
            addThreadedComment(worksheet, &quot;C2&quot;, &quot;1&quot;, author1);
            addThreadedComment(worksheet, &quot;C2&quot;, &quot;2&quot;, author1);
            addThreadedComment(worksheet, &quot;C2&quot;, &quot;3&quot;, author1);
            addThreadedComment(worksheet, &quot;C2&quot;, &quot;4&quot;, author1);
            Cell cell = worksheet.Cells.Find(&quot;4&quot;, null, findOptions);
            Assert.AreEqual(cell.Name,&quot;C2&quot;);
            workbook.Save(Constants.destPath + &quot;CellsNet47239.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet47239.xlsx&quot;);
        }
```

### See Also

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ThreadedCommentAuthorCollection indexer (2 of 2)

Gets the person who create threaded comments.

```csharp
public ThreadedCommentAuthor this[string name] { get; }
```

| Parameter | Description |
| --- | --- |
| name | The name of the author. |

### See Also

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


