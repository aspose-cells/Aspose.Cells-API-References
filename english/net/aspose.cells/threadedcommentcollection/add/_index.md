---
title: ThreadedCommentCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: ThreadedCommentCollection method. Adds a threaded comment
type: docs
url: /net/aspose.cells/threadedcommentcollection/add/
---
## ThreadedCommentCollection.Add method

Adds a threaded comment;

```csharp
public int Add(string text, ThreadedCommentAuthor author)
```

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | The text of the threaded comment. |
| author | ThreadedCommentAuthor | The author of the threaded comment |

### Examples

```csharp
// Called: workbook.Worksheets[0].Comments[0].ThreadedComments.Add(&amp;quot;asdff&amp;quot;, null);
[Test]
        public void Method_ThreadedCommentAuthor_()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Comments.Add(&quot;b1&quot;);
            workbook.Worksheets[0].Comments[0].ThreadedComments.Add(&quot;asdff&quot;, null);
            string sau = workbook.Worksheets[0].Comments[0].Author;

            workbook.Save(Constants.destPath + &quot;CellsApp2211.xlsx&quot;);
            Workbook d = new Workbook();
            d.Combine(new Workbook(Constants.destPath + &quot;CellsApp2211.xlsx&quot;));
            Assert.IsTrue(sau != d.Worksheets[1].Comments[0].Author);



        }
```

### See Also

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedCommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


