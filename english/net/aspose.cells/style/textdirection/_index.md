---
title: Style.TextDirection
second_title: Aspose.Cells for .NET API Reference
description: Style property. Represents text reading order
type: docs
url: /net/aspose.cells/style/textdirection/
---
## Style.TextDirection property

Represents text reading order.

```csharp
public TextDirectionType TextDirection { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(TextDirectionType.LeftToRight, style.TextDirection, "style.TextDirection");
private void Property_TextDirection(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            Style style = cells[1, 1].GetStyle();
            AssertHelper.AreEqual(TextDirectionType.LeftToRight, style.TextDirection, "style.TextDirection");
        }
```

### See Also

* enum [TextDirectionType](../../textdirectiontype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


