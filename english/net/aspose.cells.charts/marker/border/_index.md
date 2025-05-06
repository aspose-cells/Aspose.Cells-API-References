---
title: Marker.Border
second_title: Aspose.Cells for .NET API Reference
description: Marker property. Gets the border
type: docs
url: /net/aspose.cells.charts/marker/border/
---
## Marker.Border property

Gets the [`border`](../../../aspose.cells.drawing/line/).

```csharp
public Line Border { get; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(cpointSrc.Marker.Border.Color, cpointDest.Marker.Border.Color, info + &amp;quot;.MarkerForegroundColor&amp;quot;);
public static void Property_Border(ChartType type, ChartPoint cpointSrc, ChartPoint cpointDest, string info)
        {
            if (AssertHelper.checkNull(cpointSrc, cpointDest, info))
            {
                return;
            }
            //Patterns
            LineTest.Property_Border(cpointSrc.Border, cpointDest.Border, info + &quot;.Border&quot;);
            AreaTest.Property_Border(cpointSrc.Area, cpointDest.Area, info + &quot;.Area&quot;);
            AssertHelper.AreEqual(cpointSrc.Shadow, cpointDest.Shadow, info + &quot;.Shadow&quot;);
            AssertHelper.AreEqual(cpointSrc.Marker.MarkerStyle, cpointDest.Marker.MarkerStyle, info + &quot;.MarkerStyle&quot;);
            if (cpointSrc.Marker.MarkerStyle != ChartMarkerType.None)
            {
                AssertHelper.AreEqual(cpointSrc.Marker.Area.Formatting, cpointDest.Marker.Area.Formatting, info + &quot;.MarkerBackgroundColorSetType&quot;);
                AssertHelper.AreEqual(cpointSrc.Marker.Area.ForegroundColor, cpointDest.Marker.Area.ForegroundColor, info + &quot;.MarkerBackgroundColor&quot;);
                AssertHelper.AreEqual(cpointSrc.Marker.Border.FormattingType, cpointDest.Marker.Border.FormattingType, info + &quot;.MarkerForegroundColorSetType&quot;);
                AssertHelper.AreEqual(cpointSrc.Marker.Border.Color, cpointDest.Marker.Border.Color, info + &quot;.MarkerForegroundColor&quot;);
                AssertHelper.AreEqual(cpointSrc.Marker.MarkerSize, cpointDest.Marker.MarkerSize, info + &quot;.MarkerSize&quot;);
            }
           
            //switch (type)
            //{
            //    case ChartType.Bar:
            //    case ChartType.Scatter:
            //    case ChartType.ScatterConnectedByCurvesWithDataMarker:
            //    case ChartType.ScatterConnectedByLinesWithDataMarker:
            //    case ChartType.LineStackedWithDataMarkers:
            //    case ChartType.LineWithDataMarkers:
            //    case ChartType.Line100PercentStackedWithDataMarkers:
            //    case ChartType.RadarWithDataMarkers:
            //        AssertHelper.AreEqual(cpointSrc.MarkerForegroundColorSetType, cpointDest.MarkerForegroundColorSetType, info + &quot;.MarkerForegroundColorSetType&quot;);
            //        FormattingType temptype = cpointSrc.MarkerForegroundColorSetType;
            //        switch (temptype)
            //        {
            //            case FormattingType.Custom:
            //                AssertHelper.Property_Border(cpointSrc.MarkerForegroundColor, cpointDest.MarkerForegroundColor, info + &quot;.MarkerForegroundColor&quot;);
            //                break;
            //        }
            //        temptype = cpointSrc.MarkerBackgroundColorSetType;
            //        AssertHelper.AreEqual(cpointSrc.MarkerBackgroundColorSetType, cpointDest.MarkerBackgroundColorSetType, info + &quot;.MarkerBackgroundColorSetType&quot;);
            //        switch (temptype)
            //        {
            //            case FormattingType.Custom:
            //                AssertHelper.Property_Border(cpointSrc.MarkerBackgroundColor, cpointDest.MarkerBackgroundColor, info + &quot;.MarkerBackgroundColor&quot;);
            //                break;
            //        }

            //        AssertHelper.AreEqual(cpointSrc.MarkerSize, cpointDest.MarkerSize, info + &quot;.MarkerSize&quot;);
            //        AssertHelper.AreEqual(cpointSrc.MarkerStyle, cpointDest.MarkerStyle, info + &quot;.MarkerStyle&quot;);
            //        break;
            //}
            //DataLabels
            DataLabelsTest.Property_Border(cpointSrc.DataLabels, cpointDest.DataLabels, info + &quot;.DataLabels&quot;);
            //Options
            AssertHelper.AreEqual(cpointSrc.Explosion, cpointDest.Explosion, info + &quot;.Explosion&quot;);
        }
```

### See Also

* class [Line](../../../aspose.cells.drawing/line/)
* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


