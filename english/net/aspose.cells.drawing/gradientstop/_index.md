---
title: Class GradientStop
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.GradientStop class. Represents the gradient stop
type: docs
url: /net/aspose.cells.drawing/gradientstop/
---
## GradientStop class

Represents the gradient stop.

```csharp
public class GradientStop
```

## Properties

| Name | Description |
| --- | --- |
| [CellsColor](../../aspose.cells.drawing/gradientstop/cellscolor/) { get; } | Gets the color of this gradient stop. |
| [Position](../../aspose.cells.drawing/gradientstop/position/) { get; set; } | The position of the stop. |
| [Transparency](../../aspose.cells.drawing/gradientstop/transparency/) { get; set; } | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |

### Examples

```csharp
// Called: public static void equals(GradientStop gsSrc, GradientStop gsDest, string info)
public static void Type_GradientStop(GradientStop gsSrc, GradientStop gsDest, string info)
        {
            CellsColorTest.Type_GradientStop(gsSrc.CellsColor, gsDest.CellsColor, info + ".CellsColor");
            AssertHelper.AreEqual(gsSrc.Position, gsDest.Position, info + ".Position");
        }
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


