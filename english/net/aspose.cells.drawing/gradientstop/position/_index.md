---
title: GradientStop.Position
second_title: Aspose.Cells for .NET API Reference
description: GradientStop property. The position of the stop
type: docs
url: /net/aspose.cells.drawing/gradientstop/position/
---
## GradientStop.Position property

The position of the stop.

```csharp
public double Position { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(gsSrc.Position, gsDest.Position, info + &amp;quot;.Position&amp;quot;);
public static void Property_Position(GradientStop gsSrc, GradientStop gsDest, string info)
        {
            CellsColorTest.Property_Position(gsSrc.CellsColor, gsDest.CellsColor, info + &quot;.CellsColor&quot;);
            AssertHelper.AreEqual(gsSrc.Position, gsDest.Position, info + &quot;.Position&quot;);
        }
```

### See Also

* class [GradientStop](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


