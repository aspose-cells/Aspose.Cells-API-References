---
title: Line.Color
second_title: Aspose.Cells for .NET API Reference
description: Line property. Represents the Color of the line
type: docs
url: /net/aspose.cells.drawing/line/color/
---
## Line.Color property

Represents the Color of the line.

```csharp
public Color Color { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.equals(lineSrc.Color, lineDest.Color, info + ".Color");
public static void Property_Color(Line lineSrc, Line lineDest, string info)
        {
            if (AssertHelper.checkNull(lineSrc, lineDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(lineSrc.IsAuto, lineDest.IsAuto, info + ".IsAuto");
            AssertHelper.AreEqual(lineSrc.IsVisible, lineDest.IsVisible, info + ".IsVisible");
            if (lineSrc.IsAuto == false && lineSrc.IsVisible == true)
            {
                AssertHelper.AreEqual(lineSrc.Style, lineDest.Style, info + ".Style");
                AssertHelper.AreEqual(lineSrc.Weight, lineDest.Weight, info + ".Weight");
                AssertHelper.Property_Color(lineSrc.Color, lineDest.Color, info + ".Color");
                AssertHelper.AreEqual(lineSrc.WeightPt, lineDest.WeightPt, info + ".WeightPt");
                AssertHelper.AreEqual(lineSrc.Transparency, lineDest.Transparency, info + ".Transparency");
                AssertHelper.AreEqual(lineSrc.IsAutomaticColor, lineDest.IsAutomaticColor, info + ".IsAutomaticColor");
            }
        }
```

### See Also

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


