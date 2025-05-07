---
title: ChartPoint.Shadow
second_title: Aspose.Cells for .NET API Reference
description: ChartPoint property. True if the chartpoint has a shadow
type: docs
url: /net/aspose.cells.charts/chartpoint/shadow/
---
## ChartPoint.Shadow property

True if the chartpoint has a shadow.

```csharp
public bool Shadow { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(cpointSrc.Shadow, cpointDest.Shadow, info + ".Shadow");
public static void Property_Shadow(ChartType type, ChartPoint cpointSrc, ChartPoint cpointDest, string info)
        {
            if (AssertHelper.checkNull(cpointSrc, cpointDest, info))
            {
                return;
            }
            //Patterns
            LineTest.Property_Shadow(cpointSrc.Border, cpointDest.Border, info + ".Border");
            AreaTest.Property_Shadow(cpointSrc.Area, cpointDest.Area, info + ".Area");
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
            //                AssertHelper.Property_Shadow(cpointSrc.MarkerForegroundColor, cpointDest.MarkerForegroundColor, info + ".MarkerForegroundColor");
            //                break;
            //        }
            //        temptype = cpointSrc.MarkerBackgroundColorSetType;
            //        AssertHelper.AreEqual(cpointSrc.MarkerBackgroundColorSetType, cpointDest.MarkerBackgroundColorSetType, info + ".MarkerBackgroundColorSetType");
            //        switch (temptype)
            //        {
            //            case FormattingType.Custom:
            //                AssertHelper.Property_Shadow(cpointSrc.MarkerBackgroundColor, cpointDest.MarkerBackgroundColor, info + ".MarkerBackgroundColor");
            //                break;
            //        }

            //        AssertHelper.AreEqual(cpointSrc.MarkerSize, cpointDest.MarkerSize, info + ".MarkerSize");
            //        AssertHelper.AreEqual(cpointSrc.MarkerStyle, cpointDest.MarkerStyle, info + ".MarkerStyle");
            //        break;
            //}
            //DataLabels
            DataLabelsTest.Property_Shadow(cpointSrc.DataLabels, cpointDest.DataLabels, info + ".DataLabels");
            //Options
            AssertHelper.AreEqual(cpointSrc.Explosion, cpointDest.Explosion, info + ".Explosion");
        }
```

### See Also

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


