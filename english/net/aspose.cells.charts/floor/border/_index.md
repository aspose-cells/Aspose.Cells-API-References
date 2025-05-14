---
title: Floor.Border
second_title: Aspose.Cells for .NET API Reference
description: Floor property. Gets or sets the border Line
type: docs
url: /net/aspose.cells.charts/floor/border/
---
## Floor.Border property

Gets or sets the border [`Line`](../../../aspose.cells.drawing/line/).

```csharp
public Line Border { get; set; }
```

### Examples

```csharp
// Called: LineTest.equals(floorSrc.Border, floorDest.Border, info + ".Border");
public static void Floor_Property_Border(Floor floorSrc, Floor floorDest, string info)
        {
            if (AssertHelper.checkNull(floorSrc, floorDest, info))
            {
                return;
            }
            LineTest.Floor_Property_Border(floorSrc.Border, floorDest.Border, info + ".Border");            
            AssertHelper.AreEqual(floorSrc.Formatting, floorDest.Formatting, info + ".Formatting");
            if (floorSrc.Formatting == FormattingType.Custom)
            {
                FillFormatTest.Floor_Property_Border(floorSrc.FillFormat, floorDest.FillFormat, info + ".FillFormat");
                AssertHelper.Floor_Property_Border(floorSrc.ForegroundColor, floorDest.ForegroundColor, info + ".ForegroundColor");
                AssertHelper.Floor_Property_Border(floorSrc.BackgroundColor, floorDest.BackgroundColor, info + ".BackgroundColor");
            }
            AssertHelper.AreEqual(floorSrc.InvertIfNegative, floorDest.InvertIfNegative, info + ".InvertIfNegative");
        }
```

### See Also

* class [Line](../../../aspose.cells.drawing/line/)
* class [Floor](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


