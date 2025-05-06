---
title: Line.IsAutomaticColor
second_title: Aspose.Cells for .NET API Reference
description: Line property. Indicates whether the color of line is automatic assigned
type: docs
url: /net/aspose.cells.drawing/line/isautomaticcolor/
---
## Line.IsAutomaticColor property

Indicates whether the color of line is automatic assigned.

```csharp
public bool IsAutomaticColor { get; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(lineSrc.IsAutomaticColor, lineDest.IsAutomaticColor, info + &amp;quot;.IsAutomaticColor&amp;quot;);
public static void Property_IsAutomaticColor(Line lineSrc, Line lineDest, string info)
        {
            if (AssertHelper.checkNull(lineSrc, lineDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(lineSrc.IsAuto, lineDest.IsAuto, info + &quot;.IsAuto&quot;);
            AssertHelper.AreEqual(lineSrc.IsVisible, lineDest.IsVisible, info + &quot;.IsVisible&quot;);
            if (lineSrc.IsAuto == false &amp;&amp; lineSrc.IsVisible == true)
            {
                AssertHelper.AreEqual(lineSrc.Style, lineDest.Style, info + &quot;.Style&quot;);
                AssertHelper.AreEqual(lineSrc.Weight, lineDest.Weight, info + &quot;.Weight&quot;);
                AssertHelper.Property_IsAutomaticColor(lineSrc.Color, lineDest.Color, info + &quot;.Color&quot;);
                AssertHelper.AreEqual(lineSrc.WeightPt, lineDest.WeightPt, info + &quot;.WeightPt&quot;);
                AssertHelper.AreEqual(lineSrc.Transparency, lineDest.Transparency, info + &quot;.Transparency&quot;);
                AssertHelper.AreEqual(lineSrc.IsAutomaticColor, lineDest.IsAutomaticColor, info + &quot;.IsAutomaticColor&quot;);
            }
        }
```

### See Also

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


