---
title: DataLabels.ShowSeriesName
second_title: Aspose.Cells for .NET API Reference
description: DataLabels property. Indicates whether the series name displays for the data labels on a chart. True to show the series name. False to hide
type: docs
url: /net/aspose.cells.charts/datalabels/showseriesname/
---
## DataLabels.ShowSeriesName property

Indicates whether the series name displays for the data labels on a chart. True to show the series name. False to hide.

```csharp
public bool ShowSeriesName { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(dlabelsSrc.ShowSeriesName, dlabelsDest.ShowSeriesName, info + &amp;quot;.ShowSeriesName&amp;quot;);
public static void Property_ShowSeriesName(DataLabels dlabelsSrc, DataLabels dlabelsDest, string info)
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
            LineTest.Property_ShowSeriesName(dlabelsSrc.Border, dlabelsDest.Border, info + &quot;.Border&quot;);
            AssertHelper.AreEqual(dlabelsSrc.Shadow, dlabelsDest.Shadow, info + &quot;.Shadow&quot;);
            AreaTest.Property_ShowSeriesName(dlabelsSrc.Area, dlabelsDest.Area, info + &quot;.Area&quot;);
            //====================compare Font================//
            FontTest.Property_ShowSeriesName(dlabelsSrc.TextFont, dlabelsDest.TextFont, info + &quot;.TextFont&quot;);
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

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


