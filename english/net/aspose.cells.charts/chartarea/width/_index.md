---
title: ChartArea.Width
second_title: Aspose.Cells for .NET API Reference
description: ChartArea property. Gets or sets the horizontal offset from its lower right corner column in units of 1/4000 of the chart area
type: docs
url: /net/aspose.cells.charts/chartarea/width/
---
## ChartArea.Width property

Gets or sets the horizontal offset from its lower right corner column, in units of 1/4000 of the chart area.

```csharp
[Obsolete("Use ChartArea.WidthRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int Width { get; set; }
```

### Remarks

NOTE: This member is now obsolete. Please use ChartArea.WidthRatioToChart property, instead. Width = WidthRatioToChart * 4000. This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: AssertHelper.AreEqual(areaSrc.Width, areaDest.Width, info + &amp;quot;.Width&amp;quot;);
public static void Property_Width(ChartArea areaSrc, ChartArea areaDest, string info)
        {
            if (AssertHelper.checkNull(areaSrc, areaDest, info))
            {
                return;
            }
            //============compare patterns==============//
            //border
            AssertHelper.AreEqual(areaSrc.Border.IsAuto, areaDest.Border.IsAuto, info + &quot;.Border.IsAuto&quot;);
            AssertHelper.AreEqual(areaSrc.Border.IsVisible, areaDest.Border.IsVisible, info + &quot;.Border.IsVisible&quot;);
            if (areaSrc.Border.IsVisible == true &amp;&amp; areaSrc.Border.IsAuto == false)
            {
                //AssertHelper.AreEqual(areaSrc.Border.Style, areaDest.Border.Style, info + &quot;.Border.Style&quot;);
                //AssertHelper.Property_Width(areaSrc.Border.Color, areaDest.Border.Color, info + &quot;.Border.Color&quot;);
                //AssertHelper.AreEqual(areaSrc.Border.Weight, areaDest.Border.Weight, info + &quot;.Border.Weight&quot;);
                LineTest.Property_Width(areaSrc.Border, areaDest.Border, info+&quot;.Border&quot;);
            }
            AssertHelper.AreEqual(areaSrc.Shadow, areaDest.Shadow, info + &quot;.Shadow&quot;);
            //area
            AreaTest.Property_Width(areaSrc.Area, areaDest.Area, info + &quot;.Area&quot;);
            //==============compare font================//
            FontTest.Property_Width(areaSrc.TextFont, areaDest.TextFont, info + &quot;.TextFont&quot;);
            AssertHelper.AreEqual(areaSrc.AutoScaleFont, areaDest.AutoScaleFont, info + &quot;.AutoScaleFont&quot;);
            AssertHelper.AreEqual(areaSrc.BackgroundMode, areaDest.BackgroundMode, info + &quot;.BackgroundMode&quot;);
            //==============compare properties============//
            

            //==============compare other===============//
            AssertHelper.AreEqual(areaSrc.Height, areaDest.Height, info + &quot;.Height&quot;);
            AssertHelper.AreEqual(areaSrc.Width, areaDest.Width, info + &quot;.Width&quot;);
            ShapePropertiesTest.Property_Width(areaSrc.ShapeProperties, areaDest.ShapeProperties, info + &quot;.ShapeProperties&quot;);
            AssertHelper.AreEqual(areaSrc.IsAutomaticSize, areaDest.IsAutomaticSize, info + &quot;.IsAutomaticSize&quot;);
        }
```

### See Also

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


