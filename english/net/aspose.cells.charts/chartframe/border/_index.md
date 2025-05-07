---
title: ChartFrame.Border
second_title: Aspose.Cells for .NET API Reference
description: ChartFrame property. Gets the border
type: docs
url: /net/aspose.cells.charts/chartframe/border/
---
## ChartFrame.Border property

Gets the [`border`](../../../aspose.cells.drawing/line/).

```csharp
public virtual Line Border { get; }
```

### Examples

```csharp
// Called: LineTest.equals(cframeSrc.Border, cframeDest.Border, info + ".Border");
public static void Property_Border(ChartFrame cframeSrc, ChartFrame cframeDest, string info)
        {
            if (AssertHelper.checkNull(cframeSrc, cframeDest, info))
            {
                return;
            }
            LineTest.Property_Border(cframeSrc.Border, cframeDest.Border, info + ".Border");
            AreaTest.Property_Border(cframeSrc.Area, cframeDest.Area, info + ".Area");
            AssertHelper.AreEqual(cframeSrc.AutoScaleFont, cframeDest.AutoScaleFont, info+".AutoScaleFont");
            AssertHelper.AreEqual(cframeSrc.BackgroundMode, cframeDest.BackgroundMode, info + ".BackgroundMode");
            AssertHelper.AreEqual(cframeSrc.Height, cframeDest.Height, info + ".Height");
            AssertHelper.AreEqual(cframeSrc.Shadow, cframeDest.Shadow, info + ".Shadow");
            FontTest.Property_Border(cframeSrc.Font, cframeDest.Font, info + ".TextFont");
            AssertHelper.AreEqual(cframeSrc.Width, cframeDest.Width, info + ".Width");
            AssertHelper.AreEqual(cframeSrc.X, cframeDest.X, info + ".X");
            AssertHelper.AreEqual(cframeSrc.Y, cframeDest.Y, info + ".Y");

            AssertHelper.AreEqual(cframeSrc.IsAutomaticSize, cframeDest.IsAutomaticSize, info + ".IsAutomaticSize");
            ShapePropertiesTest.Property_Border(cframeSrc.ShapeProperties, cframeDest.ShapeProperties, info + ".ShapeProperties");
        }
```

### See Also

* class [Line](../../../aspose.cells.drawing/line/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


