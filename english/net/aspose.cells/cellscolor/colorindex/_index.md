---
title: CellsColor.ColorIndex
second_title: Aspose.Cells for .NET API Reference
description: CellsColor property. Gets and sets the color index in the color palette. Only applies of indexed color
type: docs
url: /net/aspose.cells/cellscolor/colorindex/
---
## CellsColor.ColorIndex property

Gets and sets the color index in the color palette. Only applies of indexed color.

```csharp
public int ColorIndex { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(cellsColorSrc.ColorIndex, cellsColorDest.ColorIndex, info + &amp;quot;.ColorIndex&amp;quot;);
public static void Property_ColorIndex(CellsColor cellsColorSrc, CellsColor cellsColorDest, string info)
        {
            AssertHelper.Property_ColorIndex(cellsColorSrc.Color, cellsColorDest.Color, info + &quot;.Color&quot;);
            AssertHelper.AreEqual(cellsColorSrc.ColorIndex, cellsColorDest.ColorIndex, info + &quot;.ColorIndex&quot;);

            ThemeColorTest.Property_ColorIndex(cellsColorSrc.ThemeColor, cellsColorDest.ThemeColor, info+&quot;.ThemeColor&quot;);
        }
```

### See Also

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


