---
title: ChartFrame.X
second_title: Aspose.Cells for .NET API Reference
description: ChartFrame property. Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area
type: docs
url: /net/aspose.cells.charts/chartframe/x/
---
## ChartFrame.X property

Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area.

```csharp
[Obsolete("Use ChartFrame.XRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual int X { get; set; }
```

### Remarks

How to convert units of 1/4000 to pixels? X In Pixels = X * Chart.ChartObject.Width / 4000d;

NOTE: This member is now obsolete. Please use ChartFrame.XRatioToChart property, instead. X = XRatioToChart * 4000. This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: AssertHelper.AreEqual(cframeSrc.X, cframeDest.X, info + &amp;quot;.X&amp;quot;);
public static void Property_X(ChartFrame cframeSrc, ChartFrame cframeDest, string info)
        {
            if (AssertHelper.checkNull(cframeSrc, cframeDest, info))
            {
                return;
            }
            LineTest.Property_X(cframeSrc.Border, cframeDest.Border, info + &quot;.Border&quot;);
            AreaTest.Property_X(cframeSrc.Area, cframeDest.Area, info + &quot;.Area&quot;);
            AssertHelper.AreEqual(cframeSrc.AutoScaleFont, cframeDest.AutoScaleFont, info+&quot;.AutoScaleFont&quot;);
            AssertHelper.AreEqual(cframeSrc.BackgroundMode, cframeDest.BackgroundMode, info + &quot;.BackgroundMode&quot;);
            AssertHelper.AreEqual(cframeSrc.Height, cframeDest.Height, info + &quot;.Height&quot;);
            AssertHelper.AreEqual(cframeSrc.Shadow, cframeDest.Shadow, info + &quot;.Shadow&quot;);
            FontTest.Property_X(cframeSrc.Font, cframeDest.Font, info + &quot;.TextFont&quot;);
            AssertHelper.AreEqual(cframeSrc.Width, cframeDest.Width, info + &quot;.Width&quot;);
            AssertHelper.AreEqual(cframeSrc.X, cframeDest.X, info + &quot;.X&quot;);
            AssertHelper.AreEqual(cframeSrc.Y, cframeDest.Y, info + &quot;.Y&quot;);

            AssertHelper.AreEqual(cframeSrc.IsAutomaticSize, cframeDest.IsAutomaticSize, info + &quot;.IsAutomaticSize&quot;);
            ShapePropertiesTest.Property_X(cframeSrc.ShapeProperties, cframeDest.ShapeProperties, info + &quot;.ShapeProperties&quot;);
        }
```

### See Also

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


