---
title: Line.Transparency
second_title: Aspose.Cells for .NET API Reference
description: Line property. Returns or sets the degree of transparency of the line as a value from 0.0 opaque through 1.0 clear
type: docs
url: /net/aspose.cells.drawing/line/transparency/
---
## Line.Transparency property

Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear).

```csharp
public double Transparency { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(lineSrc.Transparency, lineDest.Transparency, info + ".Transparency");
public static void Line_Property_Transparency(Line lineSrc, Line lineDest, string info)
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
                AssertHelper.Line_Property_Transparency(lineSrc.Color, lineDest.Color, info + ".Color");
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


