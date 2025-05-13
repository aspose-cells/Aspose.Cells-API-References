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
// Called: worksheet.Comments[commentIndexC2].Note = "Note for C2";
static void Worksheet_Property_Comments(Worksheet worksheet)
        {
            worksheet.Cells["A1"].PutValue("Cell A1");
            int commentIndexA1 = worksheet.Comments.Add(0, 0);
            worksheet.Comments[commentIndexA1].Note = "Note for A1";

            worksheet.Cells["B1"].PutValue("Cell B1");
            int commentIndexB1 = worksheet.Comments.Add(0, 1);
            worksheet.Comments[commentIndexB1].Note = "Note for B1";

            worksheet.Cells["C1"].PutValue("Cell C1");
            int commentIndexC1 = worksheet.Comments.Add(0, 2);
            worksheet.Comments[commentIndexC1].Note = "Note for C1";

            worksheet.Cells["A2"].PutValue("Cell A2");
            int commentIndexA2 = worksheet.Comments.Add(1, 0);
            worksheet.Comments[commentIndexA2].Note = "Note for A2";

            worksheet.Cells["B2"].PutValue("Cell B2");
            int commentIndexB2 = worksheet.Comments.Add(1, 1);
            worksheet.Comments[commentIndexB2].Note = "Note for B2";

            worksheet.Cells["C2"].PutValue("Cell C2");
            int commentIndexC2 = worksheet.Comments.Add(1, 2);
            worksheet.Comments[commentIndexC2].Note = "Note for C2";
        }
```

### See Also

* class [CommentCollection](../../commentcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


