---
title: ChartFrame.Height
second_title: Aspose.Cells for .NET API Reference
description: ChartFrame property. Gets or sets the height of frame in units of 1/4000 of the chart area
type: docs
url: /net/aspose.cells.charts/chartframe/height/
---
## ChartFrame.Height property

Gets or sets the height of frame in units of 1/4000 of the chart area.

```csharp
[Obsolete("Use ChartFrame.HeightRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual int Height { get; set; }
```

### Remarks

How to convert units of 1/4000 to pixels? Height In Pixels = Y * Chart.ChartObject.Height / 4000d;

NOTE: This member is now obsolete. Please use ChartFrame.HeightRatioToChart property, instead. Height = HeightRatioToChart * 4000. This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: AssertHelper.AreEqual(dlabelsSrc.Height, dlabelsDest.Height, info + &amp;quot;.Height&amp;quot;);
public static void Property_Height(DataLabels dlabelsSrc, DataLabels dlabelsDest, string info)
        {
            if (AssertHelper.checkNull(dlabelsSrc, dlabelsDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(dlabelsSrc.ShowSeriesName, dlabelsDest.ShowSeriesName, info + &quot;.ShowSeriesName&quot;);
            AssertHelper.AreEqual(dlabelsSrc.ShowCategoryName, dlabelsDest.ShowCategoryName, info + &quot;.ShowCategoryName&quot;);
            AssertHelper.AreEqual(dlabelsSrc.ShowValue, dlabelsDest.ShowValue, info + &quot;.ShowValue&quot;);
            AssertHelper.AreEqual(dlabelsSrc.ShowPercentage, dlabelsDest.ShowPercentage, info + &quot;.ShowPercentage&quot;);
            AssertHelper.AreEqual(dlabelsSrc.ShowBubbleSize, dlabelsDest.ShowBubbleSize, info + &quot;.ShowBubbleSize&quot;);
            AssertHelper.AreEqual(dlabelsSrc.SeparatorType, dlabelsDest.SeparatorType, info + &quot;.Separator&quot;);
            AssertHelper.AreEqual(dlabelsSrc.ShowLegendKey, dlabelsDest.ShowLegendKey, info + &quot;.ShowLegendKey&quot;);
            //====================compare Patterns================//
            LineTest.Property_Height(dlabelsSrc.Border, dlabelsDest.Border, info + &quot;.Border&quot;);
            AssertHelper.AreEqual(dlabelsSrc.Shadow, dlabelsDest.Shadow, info + &quot;.Shadow&quot;);
            AreaTest.Property_Height(dlabelsSrc.Area, dlabelsDest.Area, info + &quot;.Area&quot;);
            //====================compare Font================//
            FontTest.Property_Height(dlabelsSrc.TextFont, dlabelsDest.TextFont, info + &quot;.TextFont&quot;);
            AssertHelper.AreEqual(dlabelsSrc.AutoScaleFont, dlabelsDest.AutoScaleFont, info + &quot;.AutoScaleFont&quot;);
            AssertHelper.AreEqual(dlabelsSrc.BackgroundMode, dlabelsDest.BackgroundMode, info + &quot;.BackgroundMode&quot;);
            //====================compare Number================//
            bool lSrc = dlabelsSrc.NumberFormatLinked;
            bool lDest = dlabelsDest.NumberFormatLinked;
            AssertHelper.AreEqual(lSrc, lDest, info + &quot;.NumberFormatLinked&quot;);
            if (lSrc == false &amp;&amp; lDest == false)
            {
                AssertHelper.AreEqual(dlabelsSrc.Number, dlabelsDest.Number, info + &quot;.Number&quot;);
                AssertHelper.AreEqual(dlabelsSrc.NumberFormat, dlabelsDest.NumberFormat, info + &quot;.NumberFormat&quot;);
            }
            //====================compare Alignment================//
            AssertHelper.AreEqual(dlabelsSrc.TextHorizontalAlignment, dlabelsDest.TextHorizontalAlignment, info + &quot;.TextHorizontalAlignment&quot;);
            AssertHelper.AreEqual(dlabelsSrc.TextVerticalAlignment, dlabelsDest.TextVerticalAlignment, info + &quot;.TextVerticalAlignment&quot;);
            AssertHelper.AreEqual(dlabelsSrc.Position, dlabelsDest.Position, info + &quot;.Position&quot;);
            AssertHelper.AreEqual(dlabelsSrc.TextDirection, dlabelsDest.TextDirection, info + &quot;.TextDirection&quot;);
            AssertHelper.AreEqual(dlabelsSrc.RotationAngle, dlabelsDest.RotationAngle, info + &quot;.RotationAngle&quot;);      
            //====================compare other===================//
            AssertHelper.AreEqual(dlabelsSrc.Height, dlabelsDest.Height, info + &quot;.Height&quot;);
            AssertHelper.AreEqual(dlabelsSrc.Width, dlabelsDest.Width, info + &quot;.Width&quot;);            
        }
```

### See Also

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


