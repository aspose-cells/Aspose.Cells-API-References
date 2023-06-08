---
title: Shape.HtmlText
second_title: Aspose.Cells for .NET API Reference
description: Shape property. Gets and sets the html string which contains data and some formats in this textbox
type: docs
url: /net/aspose.cells.drawing/shape/htmltext/
---
## Shape.HtmlText property

Gets and sets the html string which contains data and some formats in this textbox.

```csharp
public string HtmlText { get; set; }
```

### Examples

```csharp

[C#]
string html = shape.HtmlText;
if(html == null || html == "")
{
    shape.HtmlText = "<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>";
}
```

### See Also

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


