---
title: Chart.Walls
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Returns a Walls object that represents the walls of a 3D chart
type: docs
url: /net/aspose.cells.charts/chart/walls/
---
## Chart.Walls property

Returns a `Walls` object that represents the walls of a 3-D chart.

```csharp
public Walls Walls { get; }
```

### Remarks

This property doesn't apply to 3-D pie charts.

### Examples

```csharp
// Called: Walls walls = chart.Walls;
        public void Chart_Property_Walls()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "Charts\\CylinderColumn.xls");
            Worksheet worksheet = workbook.Worksheets[0];
            Chart chart = worksheet.Charts[0];
            ReflectInvoker.invoke("chart", chart, new Object[][]{
			    new Object[]{"Type", ChartType.Cylinder},
                new Object[] {"IsRectangularCornered", true},
                new Object[] {"Elevation", 15},
                new Object[] { "RotationAngle", 20},
                new Object[] { "AutoScaling", true},
                new Object[] {"RightAngleAxes", true},
                new Object[] {"WallsAndGridlines2D", false},
                new Object[] { "ShowLegend", false},
                new Object[] { "ShowDataTable", false},
                new Object[] {"GapDepth", 150},
                new Object[] {"GapWidth", 10}
            });   
            ReflectInvoker.invoke("chart.ChartObject", chart.ChartObject, new Object[][]{
                new Object[] { "IsPrintable", true},
			    new Object[]{"IsLocked", true},
                new Object[] {"Placement", PlacementType.Move}});      
            
            //====================ChartArea================//
            ChartArea chartArea = chart.ChartArea;
            //AssertHelper.AreEqual(true, chartArea.Border.IsAuto, "chartArea.Border.IsAuto");
            AssertHelper.AreEqual(FormattingType.Automatic, chartArea.Area.Formatting, "chartarea.Area.Formatting");
            ReflectInvoker.invoke("chartArea", chartArea, new Object[][]{
				new Object[]{"Shadow", false},
				new Object[]{"AutoScaleFont", false},
				new Object[] { "BackgroundMode", BackgroundMode.Automatic},
			});
            ReflectInvoker.invoke("chartArea.TextFont", chartArea.TextFont, new Object[][]{
			    new Object[]{"Name", "Tahoma"},
			    new Object[]{"Size", 10},
			    new Object[]{"Underline", FontUnderlineType.None},
			    new Object[]{"Color", Color.Black},
			    new Object[]{"IsBold", false},
			    new Object[]{"IsItalic", false},
			    new Object[]{"IsStrikeout", false},
			    new Object[]{"IsSubscript", false},
                new Object[] {"IsSuperscript", false}
			});               
            //================ChartTitle===================//
            Title title = chart.Title;
            AssertHelper.AreEqual(false, title.Border.IsVisible, "title.Border.IsVisible");
            //AssertHelper.AreEqual(FormattingType.Automatic, title.Area.Formatting, "title.Area.Formatting");
            AssertHelper.AreEqual(FormattingType.None, title.Area.Formatting, "title.Area.Formatting");
            ReflectInvoker.invoke("title", title, new Object[][]{
                  new Object[] {"Text", "Number of Employees"},
                  new Object[] {"Shadow", false},
			      new Object[] {"AutoScaleFont", false},
			      new Object[] { "BackgroundMode", BackgroundMode.Automatic},
                  new Object[] {"TextHorizontalAlignment", TextAlignmentType.Center},
                  new Object[] {"TextVerticalAlignment", TextAlignmentType.Center},
                  new Object[] {"TextDirection", TextDirectionType.Context},
                  new Object[] { "RotationAngle", 0}
			});
            ReflectInvoker.invoke("title.TextFont", title.Font, new Object[][]{
			    new Object[]{"Name", "Arial"},
			    new Object[]{"Size", 11},
			    new Object[]{"Underline", FontUnderlineType.None},
			    new Object[]{"Color", Color.Black},
			    new Object[]{"IsBold", true},
			    new Object[]{"IsItalic", false},
			    new Object[]{"IsStrikeout", false},
			    new Object[]{"IsSubscript", false},
                new Object[] {"IsSuperscript", false}
			});
            //===============PlotArea===================//
            AssertHelper.AreEqual(false, chart.PlotArea.Border.IsVisible, "chart.PlotArea.Border.IsVisible");
            //AssertHelper.AreEqual(FormattingType.Automatic, chart.PlotArea.Area.Formatting, "chart.PlotArea.Area.Formatting");
            AssertHelper.AreEqual(FormattingType.Automatic, chart.PlotArea.Area.Formatting, "chart.PlotArea.Area.Formatting");
            //===============NSeries===================//
            SeriesCollection nseries = chart.NSeries;
            AssertHelper.AreEqual("='Cylinder Column'!$A$2:$A$12", nseries.CategoryData, "nseries.CategoryData");
            //================ASeries=======================//
            Series aseries = nseries[0];
            AssertHelper.AreEqual(FormattingType.Automatic, aseries.Area.Formatting, "aseries.Area.Formatting");
            AssertHelper.AreEqual(true, aseries.Area.InvertIfNegative, "aseries.Area.InvertIfNegative");
            ReflectInvoker.invoke("aseries", aseries, new Object[][]{
			    new Object[]{ "Bar3DShapeType", Bar3DShapeType.Cylinder},               
                new Object[] {"GapWidth", (short)10}
               });            
            //===========DataLabels==========================//
            DataLabels dataLabels = aseries.DataLabels;
              ReflectInvoker.invoke("dataLabels", dataLabels, new Object[][]{
			      new Object[]{ "ShowSeriesName", false},               
                  new Object[] { "ShowCategoryName", false},
                  new Object[] { "ShowValue", false},
                  new Object[] {"Separator",  DataLabelsSeparatorType.Auto}
               });
            //==============CategoryAxis====================//
            Axis categoryAxis = chart.CategoryAxis;
            ReflectInvoker.invoke("categoryAxis.AxisLine", categoryAxis.AxisLine, new Object[][]{
			    new Object[]{"Style", LineType.Solid},
			    new Object[]{"Color", Color.Empty},
			    new Object[]{"Weight",WeightType.HairLine}});

            ReflectInvoker.invoke("categoryAxis", categoryAxis, new Object[][]{
                new Object[] {"CategoryType", CategoryType.AutomaticScale},
				new Object[] {"MajorTickMark", TickMarkType.Outside},
				new Object[] {"MinorTickMark", TickMarkType.None},				
				new Object[] {"TickLabelPosition", TickLabelPositionType.Low},
				new Object[] {"TickLabelSpacing", 2},
				new Object[] {"TickMarkSpacing", 1},
				new Object[] {"IsPlotOrderReversed", false}});    

                AssertHelper.AreEqual(false, categoryAxis.MajorGridLines.IsVisible, "categoryAxis.MajorGridLines.IsVisible");
                AssertHelper.AreEqual(false, categoryAxis.MinorGridLines.IsVisible, "categoryAxis.MinorGridLines.IsVisible");

            	ReflectInvoker.invoke("categoryAxis.TickLabels", categoryAxis.TickLabels, new Object[][]{
			        new Object[]{"AutoScaleFont", false},
                    new Object[] { "BackgroundMode", BackgroundMode.Automatic},
                    new Object[] {"NumberFormatLinked", true},
                    new Object[] { "RotationAngle", -30},
                    new Object[] {"Offset", 100},
                    new Object[] {"TextDirection", TextDirectionType.Context}});

		    ReflectInvoker.invoke("categoryAxis.TickLabels.Font", categoryAxis.TickLabels.Font, new Object[][]{
			    new Object[]{"Name", "Tahoma"},
			    new Object[]{"Size", 10},
			    new Object[]{"Underline", FontUnderlineType.None},
			    new Object[]{"Color", Color.Black},
			    new Object[]{"IsBold", false},
			    new Object[]{"IsItalic", false},
			    new Object[]{"isStruckOut", false},
			    new Object[]{"IsSubscript", false},
                new Object[] {"IsSuperscript", false}});	
            //=================ValueAxis======================//
            Axis valueAxis = chart.ValueAxis;
            ReflectInvoker.invoke("valueAxis.AxisLine", valueAxis.AxisLine, new Object[][]{
			    new Object[]{"Style", LineType.Solid},
			    new Object[]{"Color", Color.Empty},
			    new Object[]{"Weight",WeightType.HairLine}});
		    ReflectInvoker.invoke("valueAxis", valueAxis, new Object[][]{
				    new Object[] {"MajorTickMark", TickMarkType.Outside},
				    new Object[] {"MinorTickMark", TickMarkType.None},
				    new Object[] {"TickLabelPosition", TickLabelPositionType.NextToAxis},
				    new Object[] {"DisplayUnit", DisplayUnitType.None},
				    new Object[] {"IsLogarithmic", false},
				    new Object[] {"IsPlotOrderReversed", false},
                    //new Object[] {"IsVisible", false
                new Object[] {"IsVisible", true
                    }                 
            });      
   
            AssertHelper.AreEqual(true, valueAxis.MajorGridLines.IsVisible, "valueAxis.MajorGridLines.IsVisible");
            AssertHelper.AreEqual(false, valueAxis.MinorGridLines.IsVisible, "valueAxis.MinorGridLines.IsVisible");

            ReflectInvoker.invoke("valueAxis.TickLabels", valueAxis.TickLabels, new Object[][]{
			    new Object[]{"AutoScaleFont", false},
                new Object[] { "BackgroundMode", BackgroundMode.Automatic},
                new Object[] {"NumberFormatLinked", true},
                new Object[] { "RotationAngle", 0},
                new Object[] {"TextDirection", TextDirectionType.Context}});	
		    ReflectInvoker.invoke("valueAxis.TickLabels.Font", valueAxis.TickLabels.Font, new Object[][]{
			    new Object[]{"Name", "Tahoma"},
			    new Object[]{"Size", 10},
			    new Object[]{"Underline", FontUnderlineType.None},
			    new Object[]{"Color", Color.Black},
			    new Object[]{"IsBold", false},
			    new Object[]{"IsItalic", false},
			    new Object[]{"IsStrikeout", false},
			    new Object[]{"IsSubscript", false},
                new Object[] {"IsSuperscript", false}});	         
            //=================Walls====================//
            Walls walls = chart.Walls;
            Console.WriteLine(walls.ForegroundColor);
            Console.WriteLine(walls.BackgroundColor);

        }
```

### See Also

* class [Walls](../../walls/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


