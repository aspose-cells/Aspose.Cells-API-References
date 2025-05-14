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
// Called: ThemeColorTest.equals(cellsColorSrc.ThemeColor, cellsColorDest.ThemeColor, info+".ThemeColor");
public static void CellsColor_Property_ThemeColor(CellsColor cellsColorSrc, CellsColor cellsColorDest, string info)
        {
            AssertHelper.CellsColor_Property_ThemeColor(cellsColorSrc.Color, cellsColorDest.Color, info + ".Color");
            AssertHelper.AreEqual(cellsColorSrc.ColorIndex, cellsColorDest.ColorIndex, info + ".ColorIndex");

            ThemeColorTest.CellsColor_Property_ThemeColor(cellsColorSrc.ThemeColor, cellsColorDest.ThemeColor, info+".ThemeColor");
        }
```

### See Also

* class [ThemeColor](../../themecolor/)
* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


