---
title: Style.Pattern
second_title: Aspose.Cells for .NET API Reference
description: Style property. Gets or sets the cell background pattern type
type: docs
url: /net/aspose.cells/style/pattern/
---
## Style.Pattern property

Gets or sets the cell background pattern type.

```csharp
public BackgroundType Pattern { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(BackgroundType.Gray50, style.Pattern, "style.Pattern");
private void Style_Property_Pattern(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            Style style = cells[1, 1].GetStyle();
            AssertHelper.AreEqual(BackgroundType.Gray50, style.Pattern, "style.Pattern");
        }
```

### See Also

* enum [BackgroundType](../../backgroundtype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


