---
title: ChartPoint.Explosion
second_title: Aspose.Cells for .NET API Reference
description: ChartPoint property. The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter
type: docs
url: /net/aspose.cells.charts/chartpoint/explosion/
---
## ChartPoint.Explosion property

The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter.

```csharp
public int Explosion { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(cpointSrc.Explosion, cpointDest.Explosion, info + ".Explosion");
public static void ChartPoint_Property_Explosion(ChartType type, ChartPoint cpointSrc, ChartPoint cpointDest, string info)
        {
            if (AssertHelper.checkNull(cpointSrc, cpointDest, info))
            {
                return;
            }
            //Patterns
            LineTest.ChartPoint_Property_Explosion(cpointSrc.Border, cpointDest.Border, info + ".Border");
            AreaTest.ChartPoint_Property_Explosion(cpointSrc.Area, cpointDest.Area, info + ".Area");
            AssertHelper.AreEqual(cpointSrc.Shadow, cpointDest.Shadow, info + ".Shadow");
            AssertHelper.AreEqual(cpointSrc.Marker.MarkerStyle, cpointDest.Marker.MarkerStyle, info + ".MarkerStyle");
            if (cpointSrc.Marker.MarkerStyle != ChartMarkerType.None)
            {
                AssertHelper.AreEqual(cpointSrc.Marker.Area.Formatting, cpointDest.Marker.Area.Formatting, info + ".MarkerBackgroundColorSetType");
                AssertHelper.AreEqual(cpointSrc.Marker.Area.ForegroundColor, cpointDest.Marker.Area.ForegroundColor, info + ".MarkerBackgroundColor");
                AssertHelper.AreEqual(cpointSrc.Marker.Border.FormattingType, cpointDest.Marker.Border.FormattingType, info + ".MarkerForegroundColorSetType");
                AssertHelper.AreEqual(cpointSrc.Marker.Border.Color, cpointDest.Marker.Border.Color, info + ".MarkerForegroundColor");
                AssertHelper.AreEqual(cpointSrc.Marker.MarkerSize, cpointDest.Marker.MarkerSize, info + ".MarkerSize");
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
            //        AssertHelper.AreEqual(cpointSrc.MarkerForegroundColorSetType, cpointDest.MarkerForegroundColorSetType, info + ".MarkerForegroundColorSetType");
            //        FormattingType temptype = cpointSrc.MarkerForegroundColorSetType;
            //        switch (temptype)
            //        {
            //            case FormattingType.Custom:
            //                AssertHelper.ChartPoint_Property_Explosion(cpointSrc.MarkerForegroundColor, cpointDest.MarkerForegroundColor, info + ".MarkerForegroundColor");
            //                break;
            //        }
            //        temptype = cpointSrc.MarkerBackgroundColorSetType;
            //        AssertHelper.AreEqual(cpointSrc.MarkerBackgroundColorSetType, cpointDest.MarkerBackgroundColorSetType, info + ".MarkerBackgroundColorSetType");
            //        switch (temptype)
            //        {
            //            case FormattingType.Custom:
            //                AssertHelper.ChartPoint_Property_Explosion(cpointSrc.MarkerBackgroundColor, cpointDest.MarkerBackgroundColor, info + ".MarkerBackgroundColor");
            //                break;
            //        }

            //        AssertHelper.AreEqual(cpointSrc.MarkerSize, cpointDest.MarkerSize, info + ".MarkerSize");
            //        AssertHelper.AreEqual(cpointSrc.MarkerStyle, cpointDest.MarkerStyle, info + ".MarkerStyle");
            //        break;
            //}
            //DataLabels
            DataLabelsTest.ChartPoint_Property_Explosion(cpointSrc.DataLabels, cpointDest.DataLabels, info + ".DataLabels");
            //Options
            AssertHelper.AreEqual(cpointSrc.Explosion, cpointDest.Explosion, info + ".Explosion");
        }
```

### See Also

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


