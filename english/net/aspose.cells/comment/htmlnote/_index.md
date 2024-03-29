---
title: Comment.HtmlNote
second_title: Aspose.Cells for .NET API Reference
description: Comment property. Gets and sets the html string which contains data and some formats in this comment
type: docs
url: /net/aspose.cells/comment/htmlnote/
---
## Comment.HtmlNote property

Gets and sets the html string which contains data and some formats in this comment.

```csharp
public string HtmlNote { get; set; }
```

### Remarks

If this is a threaded comment, the note could not be changed, otherwise MS Excel could not process it as a threaded comment.

### Examples

```csharp

[C#]
comment1.HtmlNote = "<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>";
```

### See Also

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


