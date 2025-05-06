---
title: ChartArea.Height
second_title: Aspose.Cells for .NET API Reference
description: ChartArea property. Gets or sets the vertical offset from its lower right corner row in units of 1/4000 of the chart area
type: docs
url: /net/aspose.cells.charts/chartarea/height/
---
## ChartArea.Height property

Gets or sets the vertical offset from its lower right corner row, in units of 1/4000 of the chart area.

```csharp
[Obsolete("Use ChartArea.HeightRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int Height { get; set; }
```

### Remarks

NOTE: This member is now obsolete. Please use ChartArea.HeightRatioToChart property, instead. Height = HeightRatioToChart * 4000. This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: AssertHelper.AreEqual(areaSrc.Height, areaDest.Height, info + &amp;quot;.Height&amp;quot;);
public static void Property_Height(ChartArea areaSrc, ChartArea areaDest, string info)
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
                //AssertHelper.Property_Height(areaSrc.Border.Color, areaDest.Border.Color, info + &quot;.Border.Color&quot;);
                //AssertHelper.AreEqual(areaSrc.Border.Weight, areaDest.Border.Weight, info + &quot;.Border.Weight&quot;);
                LineTest.Property_Height(areaSrc.Border, areaDest.Border, info+&quot;.Border&quot;);
            }
            AssertHelper.AreEqual(areaSrc.Shadow, areaDest.Shadow, info + &quot;.Shadow&quot;);
            //area
            AreaTest.Property_Height(areaSrc.Area, areaDest.Area, info + &quot;.Area&quot;);
            //==============compare font================//
            FontTest.Property_Height(areaSrc.TextFont, areaDest.TextFont, info + &quot;.TextFont&quot;);
            AssertHelper.AreEqual(areaSrc.AutoScaleFont, areaDest.AutoScaleFont, info + &quot;.AutoScaleFont&quot;);
            AssertHelper.AreEqual(areaSrc.BackgroundMode, areaDest.BackgroundMode, info + &quot;.BackgroundMode&quot;);
            //==============compare properties============//
            

            //==============compare other===============//
            AssertHelper.AreEqual(areaSrc.Height, areaDest.Height, info + &quot;.Height&quot;);
            AssertHelper.AreEqual(areaSrc.Width, areaDest.Width, info + &quot;.Width&quot;);
            ShapePropertiesTest.Property_Height(areaSrc.ShapeProperties, areaDest.ShapeProperties, info + &quot;.ShapeProperties&quot;);
            AssertHelper.AreEqual(areaSrc.IsAutomaticSize, areaDest.IsAutomaticSize, info + &quot;.IsAutomaticSize&quot;);
        }
```

### See Also

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


