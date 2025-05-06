---
title: Chart.Elevation
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Represents the elevation of the 3D chart view in degrees
type: docs
url: /net/aspose.cells.charts/chart/elevation/
---
## Chart.Elevation property

Represents the elevation of the 3-D chart view, in degrees.

```csharp
public int Elevation { get; set; }
```

### Remarks

The chart elevation is the height at which you view the chart, in degrees. The default is 15 for most chart types. The value of this property must be between -90 and 90, except for 3-D bar charts, where it must be between 0 and 44.

### Examples

```csharp
// Called: AssertHelper.AreEqual(chartSrc.Elevation, chartDest.Elevation, info + &amp;quot;.Elevation&amp;quot;);
public static void Property_Elevation(Chart chartSrc, Chart chartDest, string info)
        {
            if (AssertHelper.checkNull(chartSrc, chartDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(chartSrc.Type, chartDest.Type, info + &quot;.Type&quot;);
            //=======================compare ChartArea======================//
            ChartAreaTest.Property_Elevation(chartSrc.ChartArea, chartDest.ChartArea, info + &quot;.ChartArea&quot;);

            //AssertHelper.AreEqual(chartSrc.PlotAreaWithoutTickLabels, chartDest.PlotAreaWithoutTickLabels, info + &quot;.PlotAreaWithoutTickLabels&quot;);
            AssertHelper.AreEqual(chartSrc.IsRectangularCornered, chartDest.IsRectangularCornered, info + &quot;.IsRectangularCornered&quot;);
            //=======================compare PlotArea======================//
            ChartFrameTest.Property_Elevation(chartSrc.PlotArea, chartDest.PlotArea, info + &quot;.PlotArea&quot;);
            //=======================compare Legend======================//
            AssertHelper.AreEqual(chartSrc.ShowLegend, chartDest.ShowLegend, info + &quot;.ShowLegend&quot;);
            if (chartSrc.ShowLegend &amp;&amp; chartDest.ShowLegend)
                LegendTest.Property_Elevation(chartSrc.Legend, chartDest.Legend, info + &quot;.Legend&quot;);           
           //=======================compare axis=========================//
            AxisTest.Property_Elevation(chartSrc.CategoryAxis, chartDest.CategoryAxis, info + &quot;.CategoryAxis&quot;);
            AxisTest.Property_Elevation(chartSrc.ValueAxis, chartDest.ValueAxis, info + &quot;.ValueAxis&quot;);
            AxisTest.Property_Elevation(chartSrc.SeriesAxis, chartDest.SeriesAxis, info + &quot;.SeriesAxis&quot;);
            AxisTest.Property_Elevation(chartSrc.SecondCategoryAxis, chartDest.SecondCategoryAxis, info + &quot;.SecondCategoryAxis&quot;);
            AxisTest.Property_Elevation(chartSrc.SecondValueAxis, chartDest.SecondValueAxis, info + &quot;.SecondValueAxis&quot;);
            //=======================compare ASeries======================//
            NSeriesTest.Property_Elevation(chartSrc.NSeries, chartDest.NSeries, info + &quot;.NSeries&quot;);
            //====================compare options===============//
            //for column chart
            AssertHelper.AreEqual(chartSrc.GapWidth, chartDest.GapWidth, info + &quot;.GapWidth&quot;);
            //for column3d chart
            AssertHelper.AreEqual(chartSrc.GapDepth, chartDest.GapDepth, info + &quot;.GapDepth&quot;);
            AssertHelper.AreEqual(chartSrc.DepthPercent, chartDest.DepthPercent, info + &quot;.DepthPercent&quot;);
            //for pie chart
            AssertHelper.AreEqual(chartSrc.FirstSliceAngle, chartDest.FirstSliceAngle, info + &quot;.FirstSliceAngle&quot;);
            //for Bubble chart
            //AssertHelper.AreEqual(chartSrc.SizeRepresents, chartDest.SizeRepresents, info + &quot;.SizeRepresents&quot;);
            //AssertHelper.AreEqual(chartSrc.BubbleSizes, chartDest.BubbleSizes, info + &quot;.BubbleSizes&quot;);
            //AssertHelper.AreEqual(chartSrc.ShowNegativeBubbles, chartDest.ShowNegativeBubbles, info + &quot;.ShowNegativeBubbles&quot;);
            //=======================compare chart options======================//
            TitleTest.Property_Elevation(chartSrc.Title, chartDest.Title, info + &quot;.Title&quot;);
            //compare axes
            AssertHelper.AreEqual(chartSrc.CategoryAxis.CategoryType, chartDest.CategoryAxis.CategoryType, info + &quot;.CategoryAxis.CategoryType&quot;);
            AxisTest.Property_Elevation(chartSrc.SeriesAxis, chartDest.SeriesAxis, info + &quot;.SeriesAxis&quot;);
            //compare gridlines
            AssertHelper.AreEqual(chartSrc.WallsAndGridlines2D, chartDest.WallsAndGridlines2D, info + &quot;.WallsAndGridlines2D&quot;);
            //compare datatable
            AssertHelper.AreEqual(chartSrc.ShowDataTable, chartDest.ShowDataTable, info + &quot;.ShowDataTable&quot;);
            if (chartSrc.ShowDataTable &amp;&amp; chartDest.ShowDataTable)
            {
                ChartDataTableTest.Property_Elevation(chartSrc.ChartDataTable, chartDest.ChartDataTable, info + &quot;.ChartDataTable&quot;);
            }
            //=================compare for 3d================================//            
            AssertHelper.AreEqual(chartSrc.Elevation, chartDest.Elevation, info + &quot;.Elevation&quot;);
            AssertHelper.AreEqual(chartSrc.RotationAngle, chartDest.RotationAngle, info + &quot;.RotationAngle&quot;);
            AssertHelper.AreEqual(chartSrc.Perspective, chartDest.Perspective, info + &quot;.Perspective&quot;);
            AssertHelper.AreEqual(chartSrc.AutoScaling, chartDest.AutoScaling, info + &quot;.AutoScaling&quot;);
            AssertHelper.AreEqual(chartSrc.RightAngleAxes, chartDest.RightAngleAxes, info + &quot;.RightAngleAxes&quot;);
            AssertHelper.AreEqual(chartSrc.HeightPercent, chartDest.HeightPercent, info + &quot;.HeightPercent&quot;);
            WallsTest.Property_Elevation(chartSrc.Walls, chartDest.Walls, info + &quot;.Walls&quot;);
            FloorTest.Property_Elevation(chartSrc.Floor, chartDest.Floor, info + &quot;.Floor&quot;);
            
            AssertHelper.AreEqual(chartSrc.AutoScaling, chartDest.AutoScaling, info + &quot;.AutoScaling&quot;);
            AssertHelper.AreEqual(chartSrc.WallsAndGridlines2D, chartDest.WallsAndGridlines2D, info + &quot;.WallsAndGridlines2D&quot;);
            //=================compare other================================//          
            
            AssertHelper.AreEqual(chartSrc.HidePivotFieldButtons, chartDest.HidePivotFieldButtons, info + &quot;.HidePivotFieldButtons&quot;);
            //ChartShapeTest.Property_Elevation(chartSrc.ChartObject, chartDest.ChartObject, info + &quot;.ChartObject&quot;);  
            //PageSetupTest.Property_Elevation(chartSrc.PageSetup, chartDest.PageSetup, info + &quot;.PageSetup&quot;);
            AssertHelper.AreEqual(chartSrc.PivotSource, chartDest.PivotSource, info + &quot;.PivotSource&quot;);
            AssertHelper.AreEqual(chartSrc.Placement, chartDest.Placement, info + &quot;.Placement&quot;);
            AssertHelper.AreEqual(chartSrc.PlotEmptyCellsType, chartDest.PlotEmptyCellsType, info + &quot;.PlotEmptyCellsType&quot;);
            AssertHelper.AreEqual(chartSrc.PlotVisibleCells, chartDest.PlotVisibleCells, info + &quot;.PlotVisibleCells&quot;);
            AssertHelper.AreEqual(chartSrc.PrintSize, chartDest.PrintSize, info + &quot;.PrintSize&quot;);           
            //ShapesTest.Property_Elevation(chartSrc.Shapes, chartDest.Shapes, info + &quot;.Shapes&quot;);
            AssertHelper.AreEqual(chartSrc.SizeWithWindow, chartDest.SizeWithWindow, info + &quot;.SizeWithWindow&quot;);

            AssertHelper.AreEqual(chartSrc.PlotEmptyCellsType, chartDest.PlotEmptyCellsType, info + &quot;.PlotEmptyCellsType&quot;);
            AssertHelper.AreEqual(chartSrc.PlotVisibleCells, chartDest.PlotVisibleCells, info + &quot;.PlotVisibleCells&quot;);
            AssertHelper.AreEqual(chartSrc.PivotSource, chartDest.PivotSource, info + &quot;.PivotSource&quot;);
            AssertHelper.AreEqual(chartSrc.HidePivotFieldButtons, chartDest.HidePivotFieldButtons, info + &quot;.HidePivotFieldButtons&quot;);

            //chartSrc.PageSetup
            
        }
```

### See Also

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


