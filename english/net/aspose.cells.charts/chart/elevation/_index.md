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
// Called: AssertHelper.AreEqual(chartSrc.Elevation, chartDest.Elevation, info + ".Elevation");
public static void Property_Elevation(Chart chartSrc, Chart chartDest, string info)
        {
            if (AssertHelper.checkNull(chartSrc, chartDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(chartSrc.Type, chartDest.Type, info + ".Type");
            //=======================compare ChartArea======================//
            ChartAreaTest.Property_Elevation(chartSrc.ChartArea, chartDest.ChartArea, info + ".ChartArea");

            //AssertHelper.AreEqual(chartSrc.PlotAreaWithoutTickLabels, chartDest.PlotAreaWithoutTickLabels, info + ".PlotAreaWithoutTickLabels");
            AssertHelper.AreEqual(chartSrc.IsRectangularCornered, chartDest.IsRectangularCornered, info + ".IsRectangularCornered");
            //=======================compare PlotArea======================//
            ChartFrameTest.Property_Elevation(chartSrc.PlotArea, chartDest.PlotArea, info + ".PlotArea");
            //=======================compare Legend======================//
            AssertHelper.AreEqual(chartSrc.ShowLegend, chartDest.ShowLegend, info + ".ShowLegend");
            if (chartSrc.ShowLegend && chartDest.ShowLegend)
                LegendTest.Property_Elevation(chartSrc.Legend, chartDest.Legend, info + ".Legend");           
           //=======================compare axis=========================//
            AxisTest.Property_Elevation(chartSrc.CategoryAxis, chartDest.CategoryAxis, info + ".CategoryAxis");
            AxisTest.Property_Elevation(chartSrc.ValueAxis, chartDest.ValueAxis, info + ".ValueAxis");
            AxisTest.Property_Elevation(chartSrc.SeriesAxis, chartDest.SeriesAxis, info + ".SeriesAxis");
            AxisTest.Property_Elevation(chartSrc.SecondCategoryAxis, chartDest.SecondCategoryAxis, info + ".SecondCategoryAxis");
            AxisTest.Property_Elevation(chartSrc.SecondValueAxis, chartDest.SecondValueAxis, info + ".SecondValueAxis");
            //=======================compare ASeries======================//
            NSeriesTest.Property_Elevation(chartSrc.NSeries, chartDest.NSeries, info + ".NSeries");
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
            TitleTest.Property_Elevation(chartSrc.Title, chartDest.Title, info + ".Title");
            //compare axes
            AssertHelper.AreEqual(chartSrc.CategoryAxis.CategoryType, chartDest.CategoryAxis.CategoryType, info + ".CategoryAxis.CategoryType");
            AxisTest.Property_Elevation(chartSrc.SeriesAxis, chartDest.SeriesAxis, info + ".SeriesAxis");
            //compare gridlines
            AssertHelper.AreEqual(chartSrc.WallsAndGridlines2D, chartDest.WallsAndGridlines2D, info + ".WallsAndGridlines2D");
            //compare datatable
            AssertHelper.AreEqual(chartSrc.ShowDataTable, chartDest.ShowDataTable, info + ".ShowDataTable");
            if (chartSrc.ShowDataTable && chartDest.ShowDataTable)
            {
                ChartDataTableTest.Property_Elevation(chartSrc.ChartDataTable, chartDest.ChartDataTable, info + ".ChartDataTable");
            }
            //=================compare for 3d================================//            
            AssertHelper.AreEqual(chartSrc.Elevation, chartDest.Elevation, info + ".Elevation");
            AssertHelper.AreEqual(chartSrc.RotationAngle, chartDest.RotationAngle, info + ".RotationAngle");
            AssertHelper.AreEqual(chartSrc.Perspective, chartDest.Perspective, info + ".Perspective");
            AssertHelper.AreEqual(chartSrc.AutoScaling, chartDest.AutoScaling, info + ".AutoScaling");
            AssertHelper.AreEqual(chartSrc.RightAngleAxes, chartDest.RightAngleAxes, info + ".RightAngleAxes");
            AssertHelper.AreEqual(chartSrc.HeightPercent, chartDest.HeightPercent, info + ".HeightPercent");
            WallsTest.Property_Elevation(chartSrc.Walls, chartDest.Walls, info + ".Walls");
            FloorTest.Property_Elevation(chartSrc.Floor, chartDest.Floor, info + ".Floor");
            
            AssertHelper.AreEqual(chartSrc.AutoScaling, chartDest.AutoScaling, info + ".AutoScaling");
            AssertHelper.AreEqual(chartSrc.WallsAndGridlines2D, chartDest.WallsAndGridlines2D, info + ".WallsAndGridlines2D");
            //=================compare other================================//          
            
            AssertHelper.AreEqual(chartSrc.HidePivotFieldButtons, chartDest.HidePivotFieldButtons, info + ".HidePivotFieldButtons");
            //ChartShapeTest.Property_Elevation(chartSrc.ChartObject, chartDest.ChartObject, info + ".ChartObject");  
            //PageSetupTest.Property_Elevation(chartSrc.PageSetup, chartDest.PageSetup, info + ".PageSetup");
            AssertHelper.AreEqual(chartSrc.PivotSource, chartDest.PivotSource, info + ".PivotSource");
            AssertHelper.AreEqual(chartSrc.Placement, chartDest.Placement, info + ".Placement");
            AssertHelper.AreEqual(chartSrc.PlotEmptyCellsType, chartDest.PlotEmptyCellsType, info + ".PlotEmptyCellsType");
            AssertHelper.AreEqual(chartSrc.PlotVisibleCells, chartDest.PlotVisibleCells, info + ".PlotVisibleCells");
            AssertHelper.AreEqual(chartSrc.PrintSize, chartDest.PrintSize, info + ".PrintSize");           
            //ShapesTest.Property_Elevation(chartSrc.Shapes, chartDest.Shapes, info + ".Shapes");
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


