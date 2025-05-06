---
title: Worksheet.Comments
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets the Comment collection
type: docs
url: /net/aspose.cells/worksheet/comments/
---
## Worksheet.Comments property

Gets the [`Comment`](../../comment/) collection.

```csharp
public CommentCollection Comments { get; }
```

### Examples

```csharp
// Called: Comment c = workbook.Worksheets[1].Comments[0];
[Test]
        public void Property_Comments()
        {
            Workbook workbook = new Workbook();
            var sheet = workbook.Worksheets.Add(&quot;AutosizeIssue&quot;);

            var comment = sheet.Comments.Add(5, 1);
            sheet.Comments[comment].Note = @&quot;Bug Report: AutoSize Issue in Aspose
                                     Description:AutoSize functionality is not working as expected in Aspose. 
                                     When applying AutoSize to a shape, cell, or text box, the size is either not adjusting dynamically or is incorrect based on the content.&quot;;
            sheet.Comments[comment].CommentShape.TextBody.TextAlignment.AutoSize = true;
            sheet.Comments[comment].AutoSize = true;
            workbook.Save(Constants.destPath + &quot;AutosizeIssue.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot;AutosizeIssue.xls&quot;);
            Comment c = workbook.Worksheets[1].Comments[0];
            Assert.IsTrue(c.AutoSize);
        }
```

### See Also

* class [CommentCollection](../../commentcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


