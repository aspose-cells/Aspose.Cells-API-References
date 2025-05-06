---
title: Style.VerticalAlignment
second_title: Aspose.Cells for .NET API Reference
description: Style property. Gets or sets the vertical alignment type of the text in a cell
type: docs
url: /net/aspose.cells/style/verticalalignment/
---
## Style.VerticalAlignment property

Gets or sets the vertical alignment type of the text in a cell.

```csharp
public TextAlignmentType VerticalAlignment { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(TextAlignmentType.Bottom, style.VerticalAlignment, &amp;quot;style.HorizontalAlignment&amp;quot;);
private void Property_VerticalAlignment(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            Style style = cells[1, 1].GetStyle();
            AssertHelper.AreEqual(TextAlignmentType.Bottom, style.VerticalAlignment, &quot;style.HorizontalAlignment&quot;);
        }
```

### See Also

* enum [TextAlignmentType](../../textalignmenttype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


