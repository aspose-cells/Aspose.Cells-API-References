---
title: Range.ApplyStyle
second_title: Aspose.Cells for .NET API Reference
description: Range method. Applies formats for a whole range
type: docs
url: /net/aspose.cells/range/applystyle/
---
## Range.ApplyStyle method

Applies formats for a whole range.

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The style object which will be applied. |
| flag | StyleFlag | Flags which indicates applied formatting properties. |

### Remarks

Each cell in this range will contains a [`Style`](../../style/) object. So this is a memory-consuming method. Please use it carefully.

### Examples

```csharp
// Called: oRange.ApplyStyle(style, styleflag);
public void Range_Method_ApplyStyle()
{
    Workbook workbook = new Workbook();
    Style style = workbook.CreateStyle();
    style.HorizontalAlignment = TextAlignmentType.CenterAcross;
    style.VerticalAlignment = TextAlignmentType.Bottom;
    style.IsTextWrapped = true;
    Cells cells = workbook.Worksheets[0].Cells;
    cells[0, 0].PutValue("This is an autofit rows test with wrapped data that spans multiple columns");

    Aspose.Cells.Range oRange = cells.CreateRange(0, 0, 1, 4);

    StyleFlag styleflag = new StyleFlag();
    styleflag.All = true;
    oRange.ApplyStyle(style, styleflag);

    workbook.Worksheets[0].AutoFitRows();
    Assert.AreEqual(cells.GetRowHeight(0), 25.5);




}
```

### See Also

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


