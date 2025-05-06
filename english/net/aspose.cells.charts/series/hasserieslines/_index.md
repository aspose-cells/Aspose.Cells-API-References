---
title: Series.HasSeriesLines
second_title: Aspose.Cells for .NET API Reference
description: Series property. True if a stacked column chart or bar chart has series lines or if a Pie of Pie chart or Bar of Pie chart has connector lines between the two sections. Applies only to stacked column charts bar charts Pie of Pie charts or Bar of Pie charts
type: docs
url: /net/aspose.cells.charts/series/hasserieslines/
---
## Series.HasSeriesLines property

True if a stacked column chart or bar chart has series lines or if a Pie of Pie chart or Bar of Pie chart has connector lines between the two sections. Applies only to stacked column charts, bar charts, Pie of Pie charts, or Bar of Pie charts.

```csharp
public bool HasSeriesLines { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(aseriesSrc.HasSeriesLines, aseriesDest.HasSeriesLines, info + &amp;quot;.HasSeriesLines&amp;quot;);
public static void Property_HasSeriesLines(Series aseriesSrc, Series aseriesDest, string info)
        {
            if (AssertHelper.checkNull(aseriesSrc, aseriesDest, info))
            {
                return;
            }
            //===============compare patterns================//
            LineTest.Property_HasSeriesLines(aseriesSrc.Border, aseriesDest.Border, info + &quot;.Line&quot;);
            AreaTest.Property_HasSeriesLines(aseriesSrc.Area, aseriesDest.Area, info + &quot;.Area&quot;);
            AssertHelper.AreEqual(aseriesSrc.Has3DEffect, aseriesDest.Has3DEffect, info + &quot;.Has3DEffect&quot;);
            //for line chart
            AssertHelper.AreEqual(aseriesSrc.Smooth, aseriesDest.Smooth, info + &quot;.Smooth&quot;);
            AssertHelper.AreEqual(aseriesSrc.Marker.MarkerStyle, aseriesDest.Marker.MarkerStyle, info + &quot;.MarkerStyle&quot;);
            if (aseriesSrc.Marker.MarkerStyle != ChartMarkerType.Automatic &amp;&amp; aseriesSrc.Marker.MarkerStyle != ChartMarkerType.None)
            {
                AssertHelper.AreEqual(aseriesSrc.Marker.Border.FormattingType, aseriesDest.Marker.Border.FormattingType, info + &quot;.MarkerForegroundColorSetType&quot;);
                if (aseriesSrc.Marker.Border.FormattingType != ChartLineFormattingType.None)
                {
                    AssertHelper.Property_HasSeriesLines(aseriesSrc.Marker.Border.Color, aseriesDest.Marker.Border.Color, info + &quot;.MarkerForegroundColor&quot;);
                }
                AssertHelper.AreEqual(aseriesSrc.Marker.Area.Formatting, aseriesDest.Marker.Area.Formatting, info + &quot;.MarkerBackgroundColorSetType&quot;);
                if (aseriesSrc.Marker.Area.Formatting == FormattingType.Custom)
                {
                    AssertHelper.Property_HasSeriesLines(aseriesSrc.Marker.Area.ForegroundColor, aseriesDest.Marker.Area.ForegroundColor, info + &quot;.MarkerBackgroundColor&quot;);
                }
                AssertHelper.AreEqual(aseriesSrc.Marker.MarkerSize, aseriesDest.Marker.MarkerSize, info + &quot;.MarkerSize&quot;);
            }
            AssertHelper.AreEqual(aseriesSrc.Shadow, aseriesDest.Shadow, info + &quot;.Shadow&quot;);
            //===============compare Axis===========================//

            //================compare YError Bar=================//            
            ErrorBarTest.Property_HasSeriesLines(aseriesSrc.YErrorBar, aseriesDest.YErrorBar, info + &quot;.YErrorBar&quot;);
            DataLabelsTest.Property_HasSeriesLines(aseriesSrc.DataLabels, aseriesDest.DataLabels, info + &quot;.DataLabels&quot;);
            //================compare options====================//
            //for column chart
            AssertHelper.AreEqual(aseriesSrc.Overlap, aseriesDest.Overlap, info + &quot;.Overlap&quot;);
            AssertHelper.AreEqual(aseriesSrc.IsColorVaried, aseriesDest.IsColorVaried, info + &quot;.IsColorVaried&quot;);
            //for line chart
            AssertHelper.AreEqual(aseriesSrc.HasDropLines, aseriesDest.HasDropLines, info + &quot;.HasDropLines&quot;);
            AssertHelper.AreEqual(aseriesSrc.HasHiLoLines, aseriesDest.HasHiLoLines, info + &quot;.HasHiLoLines&quot;);
            AssertHelper.AreEqual(aseriesSrc.HasUpDownBars, aseriesDest.HasUpDownBars, info + &quot;.HasUpDownBars&quot;);
            //for pie chart
            AssertHelper.AreEqual(aseriesSrc.SplitType, aseriesDest.SplitType, info + &quot;.SplitType&quot;);
            AssertHelper.AreEqual(aseriesSrc.SplitValue, aseriesDest.SplitValue, info + &quot;.SplitValue&quot;);
            AssertHelper.AreEqual(aseriesSrc.SecondPlotSize, aseriesDest.SecondPlotSize, info + &quot;.SizeRepresents&quot;);
            AssertHelper.AreEqual(aseriesSrc.GapWidth, aseriesDest.GapWidth, info + &quot;.GapWidth&quot;);
            AssertHelper.AreEqual(aseriesSrc.HasSeriesLines, aseriesDest.HasSeriesLines, info + &quot;.HasSeriesLines&quot;);
            //for area chart
            AssertHelper.AreEqual(aseriesSrc.HasDropLines, aseriesDest.HasDropLines, info + &quot;.HasDropLines&quot;);
            //for Doughnut chart
            AssertHelper.AreEqual(aseriesSrc.DoughnutHoleSize, aseriesDest.DoughnutHoleSize, info + &quot;.DoughnutHoleSize&quot;);
            //==================compare shape(for Cylinder, Pyramid  and Cone chart==============//
            AssertHelper.AreEqual(aseriesSrc.Bar3DShapeType, aseriesDest.Bar3DShapeType, info + &quot;.Bar3DShapeType&quot;);

            

        }
```

### See Also

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


