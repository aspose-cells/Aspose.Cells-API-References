---
title: Chart.GapDepth
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Gets or sets the distance between the data series in a 3D chart as a percentage of the marker width. The value of this property must be between 0 and 500
type: docs
url: /net/aspose.cells.charts/chart/gapdepth/
---
## Chart.GapDepth property

Gets or sets the distance between the data series in a 3-D chart, as a percentage of the marker width. The value of this property must be between 0 and 500.

```csharp
public int GapDepth { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(chartSrc.GapDepth, chartDest.GapDepth, info + ".GapDepth");
public static void Chart_Property_GapDepth(Chart chartSrc, Chart chartDest, string info)
        {
            if (AssertHelper.checkNull(chartSrc, chartDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(chartSrc.Type, chartDest.Type, info + ".Type");
            //=======================compare ChartArea======================//
            ChartAreaTest.Chart_Property_GapDepth(chartSrc.ChartArea, chartDest.ChartArea, info + ".ChartArea");

            //AssertHelper.AreEqual(chartSrc.PlotAreaWithoutTickLabels, chartDest.PlotAreaWithoutTickLabels, info + ".PlotAreaWithoutTickLabels");
            AssertHelper.AreEqual(chartSrc.IsRectangularCornered, chartDest.IsRectangularCornered, info + ".IsRectangularCornered");
            //=======================compare PlotArea======================//
            ChartFrameTest.Chart_Property_GapDepth(chartSrc.PlotArea, chartDest.PlotArea, info + ".PlotArea");
            //=======================compare Legend======================//
            AssertHelper.AreEqual(chartSrc.ShowLegend, chartDest.ShowLegend, info + ".ShowLegend");
            if (chartSrc.ShowLegend && chartDest.ShowLegend)
                LegendTest.Chart_Property_GapDepth(chartSrc.Legend, chartDest.Legend, info + ".Legend");           
           //=======================compare axis=========================//
            AxisTest.Chart_Property_GapDepth(chartSrc.CategoryAxis, chartDest.CategoryAxis, info + ".CategoryAxis");
            AxisTest.Chart_Property_GapDepth(chartSrc.ValueAxis, chartDest.ValueAxis, info + ".ValueAxis");
            AxisTest.Chart_Property_GapDepth(chartSrc.SeriesAxis, chartDest.SeriesAxis, info + ".SeriesAxis");
            AxisTest.Chart_Property_GapDepth(chartSrc.SecondCategoryAxis, chartDest.SecondCategoryAxis, info + ".SecondCategoryAxis");
            AxisTest.Chart_Property_GapDepth(chartSrc.SecondValueAxis, chartDest.SecondValueAxis, info + ".SecondValueAxis");
            //=======================compare ASeries======================//
            NSeriesTest.Chart_Property_GapDepth(chartSrc.NSeries, chartDest.NSeries, info + ".NSeries");
            //====================compare options===============//
            //for column chart
            AssertHelper.AreEqual(chartSrc.GapWidth, chartDest.GapWidth, info + ".GapWidth");
            //for column3d chart
            AssertHelper.AreEqual(chartSrc.GapDepth, chartDest.GapDepth, info + ".GapDepth");
            AssertHelper.AreEqual(chartSrc.DepthPercent, chartDest.DepthPercent, info + ".DepthPercent");
            //for pie chart
            AssertHelper.AreEqual(chartSrc.FirstSliceAngle, chartDest.FirstSliceAngle, info + ".FirstSliceAngle");
            //for Bubble chart
            //AssertHelper.AreEqual(chartSrc.SizeRepresents, chartDest.SizeRepresents, info + ".SizeRepresents");
            //AssertHelper.AreEqual(chartSrc.BubbleSizes, chartDest.BubbleSizes, info + ".BubbleSizes");
            //AssertHelper.AreEqual(chartSrc.ShowNegativeBubbles, chartDest.ShowNegativeBubbles, info + ".ShowNegativeBubbles");
            //=======================compare chart options======================//
            TitleTest.Chart_Property_GapDepth(chartSrc.Title, chartDest.Title, info + ".Title");
            //compare axes
            AssertHelper.AreEqual(chartSrc.CategoryAxis.CategoryType, chartDest.CategoryAxis.CategoryType, info + ".CategoryAxis.CategoryType");
            AxisTest.Chart_Property_GapDepth(chartSrc.SeriesAxis, chartDest.SeriesAxis, info + ".SeriesAxis");
            //compare gridlines
            AssertHelper.AreEqual(chartSrc.WallsAndGridlines2D, chartDest.WallsAndGridlines2D, info + ".WallsAndGridlines2D");
            //compare datatable
            AssertHelper.AreEqual(chartSrc.ShowDataTable, chartDest.ShowDataTable, info + ".ShowDataTable");
            if (chartSrc.ShowDataTable && chartDest.ShowDataTable)
            {
                ChartDataTableTest.Chart_Property_GapDepth(chartSrc.ChartDataTable, chartDest.ChartDataTable, info + ".ChartDataTable");
            }
            //=================compare for 3d================================//            
            AssertHelper.AreEqual(chartSrc.Elevation, chartDest.Elevation, info + ".Elevation");
            AssertHelper.AreEqual(chartSrc.RotationAngle, chartDest.RotationAngle, info + ".RotationAngle");
            AssertHelper.AreEqual(chartSrc.Perspective, chartDest.Perspective, info + ".Perspective");
            AssertHelper.AreEqual(chartSrc.AutoScaling, chartDest.AutoScaling, info + ".AutoScaling");
            AssertHelper.AreEqual(chartSrc.RightAngleAxes, chartDest.RightAngleAxes, info + ".RightAngleAxes");
            AssertHelper.AreEqual(chartSrc.HeightPercent, chartDest.HeightPercent, info + ".HeightPercent");
            WallsTest.Chart_Property_GapDepth(chartSrc.Walls, chartDest.Walls, info + ".Walls");
            FloorTest.Chart_Property_GapDepth(chartSrc.Floor, chartDest.Floor, info + ".Floor");
            
            AssertHelper.AreEqual(chartSrc.AutoScaling, chartDest.AutoScaling, info + ".AutoScaling");
            AssertHelper.AreEqual(chartSrc.WallsAndGridlines2D, chartDest.WallsAndGridlines2D, info + ".WallsAndGridlines2D");
            //=================compare other================================//          
            
            AssertHelper.AreEqual(chartSrc.HidePivotFieldButtons, chartDest.HidePivotFieldButtons, info + ".HidePivotFieldButtons");
            //ChartShapeTest.Chart_Property_GapDepth(chartSrc.ChartObject, chartDest.ChartObject, info + ".ChartObject");  
            //PageSetupTest.Chart_Property_GapDepth(chartSrc.PageSetup, chartDest.PageSetup, info + ".PageSetup");
            AssertHelper.AreEqual(chartSrc.PivotSource, chartDest.PivotSource, info + ".PivotSource");
            AssertHelper.AreEqual(chartSrc.Placement, chartDest.Placement, info + ".Placement");
            AssertHelper.AreEqual(chartSrc.PlotEmptyCellsType, chartDest.PlotEmptyCellsType, info + ".PlotEmptyCellsType");
            AssertHelper.AreEqual(chartSrc.PlotVisibleCells, chartDest.PlotVisibleCells, info + ".PlotVisibleCells");
            AssertHelper.AreEqual(chartSrc.PrintSize, chartDest.PrintSize, info + ".PrintSize");           
            //ShapesTest.Chart_Property_GapDepth(chartSrc.Shapes, chartDest.Shapes, info + ".Shapes");
            AssertHelper.AreEqual(chartSrc.SizeWithWindow, chartDest.SizeWithWindow, info + ".SizeWithWindow");

            AssertHelper.AreEqual(chartSrc.PlotEmptyCellsType, chartDest.PlotEmptyCellsType, info + ".PlotEmptyCellsType");
            AssertHelper.AreEqual(chartSrc.PlotVisibleCells, chartDest.PlotVisibleCells, info + ".PlotVisibleCells");
            AssertHelper.AreEqual(chartSrc.PivotSource, chartDest.PivotSource, info + ".PivotSource");
            AssertHelper.AreEqual(chartSrc.HidePivotFieldButtons, chartDest.HidePivotFieldButtons, info + ".HidePivotFieldButtons");

            //chartSrc.PageSetup
            
        }
```

### See Also

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


