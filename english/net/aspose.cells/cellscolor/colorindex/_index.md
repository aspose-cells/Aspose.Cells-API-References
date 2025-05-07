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
// Called: AssertHelper.AreEqual(cellsColorSrc.ColorIndex, cellsColorDest.ColorIndex, info + ".ColorIndex");
public static void Property_ColorIndex(CellsColor cellsColorSrc, CellsColor cellsColorDest, string info)
        {
            AssertHelper.Property_ColorIndex(cellsColorSrc.Color, cellsColorDest.Color, info + ".Color");
            AssertHelper.AreEqual(cellsColorSrc.ColorIndex, cellsColorDest.ColorIndex, info + ".ColorIndex");

            ThemeColorTest.Property_ColorIndex(cellsColorSrc.ThemeColor, cellsColorDest.ThemeColor, info+".ThemeColor");
        }
```

### See Also

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


