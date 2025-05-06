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
// Called: authors.Add(&amp;quot;Aspose&amp;quot;, &amp;quot;S::johnson.shi@asposenj.onmicrosoft.com::bd07c1a8-5f37-4ecf-bd20-1f831c9015ce&amp;quot;, &amp;quot;AD&amp;quot;);
[Test]
        public void Method_String_()
        {
            Workbook workbook = new Workbook();
            ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;
            authors.Add(&quot;Aspose&quot;, &quot;S::johnson.shi@asposenj.onmicrosoft.com::bd07c1a8-5f37-4ecf-bd20-1f831c9015ce&quot;, &quot;AD&quot;);
            authors.CurrentPerson = authors[0];


            CommentCollection comments = workbook.Worksheets[0].Comments;
            comments.AddThreadedComment(&quot;B3&quot;, &quot;Test1&quot;, null);
            comments.AddThreadedComment(&quot;B3&quot;, &quot;Test2&quot;, null);
            comments.AddThreadedComment(&quot;B3&quot;, &quot;Test3&quot;, null);
            workbook.Worksheets.Add();
            comments = workbook.Worksheets[1].Comments;
            comments.AddThreadedComment(&quot;B3&quot;, &quot;Test11&quot;, null);
            comments.AddThreadedComment(&quot;B3&quot;, &quot;Test12&quot;, null);
            comments.AddThreadedComment(&quot;B3&quot;, &quot;Test13&quot;, null);
            workbook.Save(Constants.destPath + &quot;CELLSNET46656_002.xlsx&quot;);
        }
```

### See Also

* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


