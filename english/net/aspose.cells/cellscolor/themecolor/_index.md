---
title: CellsColor.ThemeColor
second_title: Aspose.Cells for .NET API Reference
description: CellsColor property. Gets the theme color. Only applies for theme color type
type: docs
url: /net/aspose.cells/cellscolor/themecolor/
---
## CellsColor.ThemeColor property

Gets the theme color. Only applies for theme color type.

```csharp
public ThemeColor ThemeColor { get; set; }
```

### Examples

```csharp
// Called: ThemeColorTest.equals(cellsColorSrc.ThemeColor, cellsColorDest.ThemeColor, info+&amp;quot;.ThemeColor&amp;quot;);
public static void Property_ThemeColor(CellsColor cellsColorSrc, CellsColor cellsColorDest, string info)
        {
            AssertHelper.Property_ThemeColor(cellsColorSrc.Color, cellsColorDest.Color, info + &quot;.Color&quot;);
            AssertHelper.AreEqual(cellsColorSrc.ColorIndex, cellsColorDest.ColorIndex, info + &quot;.ColorIndex&quot;);

            ThemeColorTest.Property_ThemeColor(cellsColorSrc.ThemeColor, cellsColorDest.ThemeColor, info+&quot;.ThemeColor&quot;);
        }
```

### See Also

* class [ThemeColor](../../themecolor/)
* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


