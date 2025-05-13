---
title: ChartFrame.Width
second_title: Aspose.Cells for .NET API Reference
description: ChartFrame property. Gets or sets the width of frame in units of 1/4000 of the chart area
type: docs
url: /net/aspose.cells.charts/chartframe/width/
---
## ChartFrame.Width property

Gets or sets the width of frame in units of 1/4000 of the chart area.

```csharp
[Obsolete("Use ChartFrame.WidthRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual int Width { get; set; }
```

### Remarks

How to convert units of 1/4000 to pixels? Width In Pixels = Width * Chart.ChartObject.Height / 4000d;

NOTE: This member is now obsolete. Please use ChartFrame.WidthRatioToChart property, instead. Width = WidthRatioToChart * 4000; This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: AssertHelper.AreEqual(cframeSrc.Width, cframeDest.Width, info + ".Width");
public static void ChartFrame_Property_Width(ChartFrame cframeSrc, ChartFrame cframeDest, string info)
        {
            if (AssertHelper.checkNull(cframeSrc, cframeDest, info))
            {
                return;
            }
            LineTest.ChartFrame_Property_Width(cframeSrc.Border, cframeDest.Border, info + ".Border");
            AreaTest.ChartFrame_Property_Width(cframeSrc.Area, cframeDest.Area, info + ".Area");
            AssertHelper.AreEqual(cframeSrc.AutoScaleFont, cframeDest.AutoScaleFont, info+".AutoScaleFont");
            AssertHelper.AreEqual(cframeSrc.BackgroundMode, cframeDest.BackgroundMode, info + ".BackgroundMode");
            AssertHelper.AreEqual(cframeSrc.Height, cframeDest.Height, info + ".Height");
            AssertHelper.AreEqual(cframeSrc.Shadow, cframeDest.Shadow, info + ".Shadow");
            FontTest.ChartFrame_Property_Width(cframeSrc.Font, cframeDest.Font, info + ".TextFont");
            AssertHelper.AreEqual(cframeSrc.Width, cframeDest.Width, info + ".Width");
            AssertHelper.AreEqual(cframeSrc.X, cframeDest.X, info + ".X");
            AssertHelper.AreEqual(cframeSrc.Y, cframeDest.Y, info + ".Y");

            AssertHelper.AreEqual(cframeSrc.IsAutomaticSize, cframeDest.IsAutomaticSize, info + ".IsAutomaticSize");
            ShapePropertiesTest.ChartFrame_Property_Width(cframeSrc.ShapeProperties, cframeDest.ShapeProperties, info + ".ShapeProperties");
        }
```

### See Also

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


