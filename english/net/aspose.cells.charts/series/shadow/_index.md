---
title: Series.Shadow
second_title: Aspose.Cells for .NET API Reference
description: Series property. True if the series has a shadow
type: docs
url: /net/aspose.cells.charts/series/shadow/
---
## Series.Shadow property

True if the series has a shadow.

```csharp
public bool Shadow { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(aseriesSrc.Shadow, aseriesDest.Shadow, info + ".Shadow");
public static void Series_Property_Shadow(Series aseriesSrc, Series aseriesDest, string info)
        {
            if (AssertHelper.checkNull(aseriesSrc, aseriesDest, info))
            {
                return;
            }
            //===============compare patterns================//
            LineTest.Series_Property_Shadow(aseriesSrc.Border, aseriesDest.Border, info + ".Line");
            AreaTest.Series_Property_Shadow(aseriesSrc.Area, aseriesDest.Area, info + ".Area");
            AssertHelper.AreEqual(aseriesSrc.Has3DEffect, aseriesDest.Has3DEffect, info + ".Has3DEffect");
            //for line chart
            AssertHelper.AreEqual(aseriesSrc.Smooth, aseriesDest.Smooth, info + ".Smooth");
            AssertHelper.AreEqual(aseriesSrc.Marker.MarkerStyle, aseriesDest.Marker.MarkerStyle, info + ".MarkerStyle");
            if (aseriesSrc.Marker.MarkerStyle != ChartMarkerType.Automatic && aseriesSrc.Marker.MarkerStyle != ChartMarkerType.None)
            {
                AssertHelper.AreEqual(aseriesSrc.Marker.Border.FormattingType, aseriesDest.Marker.Border.FormattingType, info + ".MarkerForegroundColorSetType");
                if (aseriesSrc.Marker.Border.FormattingType != ChartLineFormattingType.None)
                {
                    AssertHelper.Series_Property_Shadow(aseriesSrc.Marker.Border.Color, aseriesDest.Marker.Border.Color, info + ".MarkerForegroundColor");
                }
                AssertHelper.AreEqual(aseriesSrc.Marker.Area.Formatting, aseriesDest.Marker.Area.Formatting, info + ".MarkerBackgroundColorSetType");
                if (aseriesSrc.Marker.Area.Formatting == FormattingType.Custom)
                {
                    AssertHelper.Series_Property_Shadow(aseriesSrc.Marker.Area.ForegroundColor, aseriesDest.Marker.Area.ForegroundColor, info + ".MarkerBackgroundColor");
                }
                AssertHelper.AreEqual(aseriesSrc.Marker.MarkerSize, aseriesDest.Marker.MarkerSize, info + ".MarkerSize");
            }
            AssertHelper.AreEqual(aseriesSrc.Shadow, aseriesDest.Shadow, info + ".Shadow");
            //===============compare Axis===========================//

            //================compare YError Bar=================//            
            ErrorBarTest.Series_Property_Shadow(aseriesSrc.YErrorBar, aseriesDest.YErrorBar, info + ".YErrorBar");
            DataLabelsTest.Series_Property_Shadow(aseriesSrc.DataLabels, aseriesDest.DataLabels, info + ".DataLabels");
            //================compare options====================//
            //for column chart
            AssertHelper.AreEqual(aseriesSrc.Overlap, aseriesDest.Overlap, info + ".Overlap");
            AssertHelper.AreEqual(aseriesSrc.IsColorVaried, aseriesDest.IsColorVaried, info + ".IsColorVaried");
            //for line chart
            AssertHelper.AreEqual(aseriesSrc.HasDropLines, aseriesDest.HasDropLines, info + ".HasDropLines");
            AssertHelper.AreEqual(aseriesSrc.HasHiLoLines, aseriesDest.HasHiLoLines, info + ".HasHiLoLines");
            AssertHelper.AreEqual(aseriesSrc.HasUpDownBars, aseriesDest.HasUpDownBars, info + ".HasUpDownBars");
            //for pie chart
            AssertHelper.AreEqual(aseriesSrc.SplitType, aseriesDest.SplitType, info + ".SplitType");
            AssertHelper.AreEqual(aseriesSrc.SplitValue, aseriesDest.SplitValue, info + ".SplitValue");
            AssertHelper.AreEqual(aseriesSrc.SecondPlotSize, aseriesDest.SecondPlotSize, info + ".SizeRepresents");
            AssertHelper.AreEqual(aseriesSrc.GapWidth, aseriesDest.GapWidth, info + ".GapWidth");
            AssertHelper.AreEqual(aseriesSrc.HasSeriesLines, aseriesDest.HasSeriesLines, info + ".HasSeriesLines");
            //for area chart
            AssertHelper.AreEqual(aseriesSrc.HasDropLines, aseriesDest.HasDropLines, info + ".HasDropLines");
            //for Doughnut chart
            AssertHelper.AreEqual(aseriesSrc.DoughnutHoleSize, aseriesDest.DoughnutHoleSize, info + ".DoughnutHoleSize");
            //==================compare shape(for Cylinder, Pyramid  and Cone chart==============//
            AssertHelper.AreEqual(aseriesSrc.Bar3DShapeType, aseriesDest.Bar3DShapeType, info + ".Bar3DShapeType");

            

        }
```

### See Also

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


