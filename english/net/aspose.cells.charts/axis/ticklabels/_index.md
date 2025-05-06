---
title: Axis.TickLabels
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Returns a TickLabels object that represents the tickmark labels for the specified axis
type: docs
url: /net/aspose.cells.charts/axis/ticklabels/
---
## Axis.TickLabels property

Returns a `TickLabels` object that represents the tick-mark labels for the specified axis.

```csharp
public TickLabels TickLabels { get; }
```

### Examples

```csharp
// Called: ReflectInvoker.invoke(&amp;quot;valueAxis.TickLabels&amp;quot;, valueAxis.TickLabels, new Object[][]{
[Test]
        public void Property_TickLabels()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Charts\\CylinderColumn.xls&quot;);
            Worksheet worksheet = workbook.Worksheets[0];
            Chart chart = worksheet.Charts[0];
            ReflectInvoker.invoke(&quot;chart&quot;, chart, new Object[][]{
			    new Object[]{&quot;Type&quot;, ChartType.Cylinder},
                new Object[] {&quot;IsRectangularCornered&quot;, true},
                new Object[] {&quot;Elevation&quot;, 15},
                new Object[] { &quot;RotationAngle&quot;, 20},
                new Object[] { &quot;AutoScaling&quot;, true},
                new Object[] {&quot;RightAngleAxes&quot;, true},
                new Object[] {&quot;WallsAndGridlines2D&quot;, false},
                new Object[] { &quot;ShowLegend&quot;, false},
                new Object[] { &quot;ShowDataTable&quot;, false},
                new Object[] {&quot;GapDepth&quot;, 150},
                new Object[] {&quot;GapWidth&quot;, 10}
            });   
            ReflectInvoker.invoke(&quot;chart.ChartObject&quot;, chart.ChartObject, new Object[][]{
                new Object[] { &quot;IsPrintable&quot;, true},
			    new Object[]{&quot;IsLocked&quot;, true},
                new Object[] {&quot;Placement&quot;, PlacementType.Move}});      
            
            //====================ChartArea================//
            ChartArea chartArea = chart.ChartArea;
            //AssertHelper.AreEqual(true, chartArea.Border.IsAuto, &quot;chartArea.Border.IsAuto&quot;);
            AssertHelper.AreEqual(FormattingType.Automatic, chartArea.Area.Formatting, &quot;chartarea.Area.Formatting&quot;);
            ReflectInvoker.invoke(&quot;chartArea&quot;, chartArea, new Object[][]{
				new Object[]{&quot;Shadow&quot;, false},
				new Object[]{&quot;AutoScaleFont&quot;, false},
				new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic},
			});
            ReflectInvoker.invoke(&quot;chartArea.TextFont&quot;, chartArea.TextFont, new Object[][]{
			    new Object[]{&quot;Name&quot;, &quot;Tahoma&quot;},
			    new Object[]{&quot;Size&quot;, 10},
			    new Object[]{&quot;Underline&quot;, FontUnderlineType.None},
			    new Object[]{&quot;Color&quot;, Color.Black},
			    new Object[]{&quot;IsBold&quot;, false},
			    new Object[]{&quot;IsItalic&quot;, false},
			    new Object[]{&quot;IsStrikeout&quot;, false},
			    new Object[]{&quot;IsSubscript&quot;, false},
                new Object[] {&quot;IsSuperscript&quot;, false}
			});               
            //================ChartTitle===================//
            Title title = chart.Title;
            AssertHelper.AreEqual(false, title.Border.IsVisible, &quot;title.Border.IsVisible&quot;);
            //AssertHelper.AreEqual(FormattingType.Automatic, title.Area.Formatting, &quot;title.Area.Formatting&quot;);
            AssertHelper.AreEqual(FormattingType.None, title.Area.Formatting, &quot;title.Area.Formatting&quot;);
            ReflectInvoker.invoke(&quot;title&quot;, title, new Object[][]{
                  new Object[] {&quot;Text&quot;, &quot;Number of Employees&quot;},
                  new Object[] {&quot;Shadow&quot;, false},
			      new Object[] {&quot;AutoScaleFont&quot;, false},
			      new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic},
                  new Object[] {&quot;TextHorizontalAlignment&quot;, TextAlignmentType.Center},
                  new Object[] {&quot;TextVerticalAlignment&quot;, TextAlignmentType.Center},
                  new Object[] {&quot;TextDirection&quot;, TextDirectionType.Context},
                  new Object[] { &quot;RotationAngle&quot;, 0}
			});
            ReflectInvoker.invoke(&quot;title.TextFont&quot;, title.Font, new Object[][]{
			    new Object[]{&quot;Name&quot;, &quot;Arial&quot;},
			    new Object[]{&quot;Size&quot;, 11},
			    new Object[]{&quot;Underline&quot;, FontUnderlineType.None},
			    new Object[]{&quot;Color&quot;, Color.Black},
			    new Object[]{&quot;IsBold&quot;, true},
			    new Object[]{&quot;IsItalic&quot;, false},
			    new Object[]{&quot;IsStrikeout&quot;, false},
			    new Object[]{&quot;IsSubscript&quot;, false},
                new Object[] {&quot;IsSuperscript&quot;, false}
			});
            //===============PlotArea===================//
            AssertHelper.AreEqual(false, chart.PlotArea.Border.IsVisible, &quot;chart.PlotArea.Border.IsVisible&quot;);
            //AssertHelper.AreEqual(FormattingType.Automatic, chart.PlotArea.Area.Formatting, &quot;chart.PlotArea.Area.Formatting&quot;);
            AssertHelper.AreEqual(FormattingType.Automatic, chart.PlotArea.Area.Formatting, &quot;chart.PlotArea.Area.Formatting&quot;);
            //===============NSeries===================//
            SeriesCollection nseries = chart.NSeries;
            AssertHelper.AreEqual(&quot;=&apos;Cylinder Column&apos;!$A$2:$A$12&quot;, nseries.CategoryData, &quot;nseries.CategoryData&quot;);
            //================ASeries=======================//
            Series aseries = nseries[0];
            AssertHelper.AreEqual(FormattingType.Automatic, aseries.Area.Formatting, &quot;aseries.Area.Formatting&quot;);
            AssertHelper.AreEqual(true, aseries.Area.InvertIfNegative, &quot;aseries.Area.InvertIfNegative&quot;);
            ReflectInvoker.invoke(&quot;aseries&quot;, aseries, new Object[][]{
			    new Object[]{ &quot;Bar3DShapeType&quot;, Bar3DShapeType.Cylinder},               
                new Object[] {&quot;GapWidth&quot;, (short)10}
               });            
            //===========DataLabels==========================//
            DataLabels dataLabels = aseries.DataLabels;
              ReflectInvoker.invoke(&quot;dataLabels&quot;, dataLabels, new Object[][]{
			      new Object[]{ &quot;ShowSeriesName&quot;, false},               
                  new Object[] { &quot;ShowCategoryName&quot;, false},
                  new Object[] { &quot;ShowValue&quot;, false},
                  new Object[] {&quot;Separator&quot;,  DataLabelsSeparatorType.Auto}
               });
            //==============CategoryAxis====================//
            Axis categoryAxis = chart.CategoryAxis;
            ReflectInvoker.invoke(&quot;categoryAxis.AxisLine&quot;, categoryAxis.AxisLine, new Object[][]{
			    new Object[]{&quot;Style&quot;, LineType.Solid},
			    new Object[]{&quot;Color&quot;, Color.Empty},
			    new Object[]{&quot;Weight&quot;,WeightType.HairLine}});

            ReflectInvoker.invoke(&quot;categoryAxis&quot;, categoryAxis, new Object[][]{
                new Object[] {&quot;CategoryType&quot;, CategoryType.AutomaticScale},
				new Object[] {&quot;MajorTickMark&quot;, TickMarkType.Outside},
				new Object[] {&quot;MinorTickMark&quot;, TickMarkType.None},				
				new Object[] {&quot;TickLabelPosition&quot;, TickLabelPositionType.Low},
				new Object[] {&quot;TickLabelSpacing&quot;, 2},
				new Object[] {&quot;TickMarkSpacing&quot;, 1},
				new Object[] {&quot;IsPlotOrderReversed&quot;, false}});    

                AssertHelper.AreEqual(false, categoryAxis.MajorGridLines.IsVisible, &quot;categoryAxis.MajorGridLines.IsVisible&quot;);
                AssertHelper.AreEqual(false, categoryAxis.MinorGridLines.IsVisible, &quot;categoryAxis.MinorGridLines.IsVisible&quot;);

            	ReflectInvoker.invoke(&quot;categoryAxis.TickLabels&quot;, categoryAxis.TickLabels, new Object[][]{
			        new Object[]{&quot;AutoScaleFont&quot;, false},
                    new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic},
                    new Object[] {&quot;NumberFormatLinked&quot;, true},
                    new Object[] { &quot;RotationAngle&quot;, -30},
                    new Object[] {&quot;Offset&quot;, 100},
                    new Object[] {&quot;TextDirection&quot;, TextDirectionType.Context}});

		    ReflectInvoker.invoke(&quot;categoryAxis.TickLabels.Font&quot;, categoryAxis.TickLabels.Font, new Object[][]{
			    new Object[]{&quot;Name&quot;, &quot;Tahoma&quot;},
			    new Object[]{&quot;Size&quot;, 10},
			    new Object[]{&quot;Underline&quot;, FontUnderlineType.None},
			    new Object[]{&quot;Color&quot;, Color.Black},
			    new Object[]{&quot;IsBold&quot;, false},
			    new Object[]{&quot;IsItalic&quot;, false},
			    new Object[]{&quot;isStruckOut&quot;, false},
			    new Object[]{&quot;IsSubscript&quot;, false},
                new Object[] {&quot;IsSuperscript&quot;, false}});	
            //=================ValueAxis======================//
            Axis valueAxis = chart.ValueAxis;
            ReflectInvoker.invoke(&quot;valueAxis.AxisLine&quot;, valueAxis.AxisLine, new Object[][]{
			    new Object[]{&quot;Style&quot;, LineType.Solid},
			    new Object[]{&quot;Color&quot;, Color.Empty},
			    new Object[]{&quot;Weight&quot;,WeightType.HairLine}});
		    ReflectInvoker.invoke(&quot;valueAxis&quot;, valueAxis, new Object[][]{
				    new Object[] {&quot;MajorTickMark&quot;, TickMarkType.Outside},
				    new Object[] {&quot;MinorTickMark&quot;, TickMarkType.None},
				    new Object[] {&quot;TickLabelPosition&quot;, TickLabelPositionType.NextToAxis},
				    new Object[] {&quot;DisplayUnit&quot;, DisplayUnitType.None},
				    new Object[] {&quot;IsLogarithmic&quot;, false},
				    new Object[] {&quot;IsPlotOrderReversed&quot;, false},
                    //new Object[] {&quot;IsVisible&quot;, false
                new Object[] {&quot;IsVisible&quot;, true
                    }                 
            });      
   
            AssertHelper.AreEqual(true, valueAxis.MajorGridLines.IsVisible, &quot;valueAxis.MajorGridLines.IsVisible&quot;);
            AssertHelper.AreEqual(false, valueAxis.MinorGridLines.IsVisible, &quot;valueAxis.MinorGridLines.IsVisible&quot;);

            ReflectInvoker.invoke(&quot;valueAxis.TickLabels&quot;, valueAxis.TickLabels, new Object[][]{
			    new Object[]{&quot;AutoScaleFont&quot;, false},
                new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic},
                new Object[] {&quot;NumberFormatLinked&quot;, true},
                new Object[] { &quot;RotationAngle&quot;, 0},
                new Object[] {&quot;TextDirection&quot;, TextDirectionType.Context}});	
		    ReflectInvoker.invoke(&quot;valueAxis.TickLabels.Font&quot;, valueAxis.TickLabels.Font, new Object[][]{
			    new Object[]{&quot;Name&quot;, &quot;Tahoma&quot;},
			    new Object[]{&quot;Size&quot;, 10},
			    new Object[]{&quot;Underline&quot;, FontUnderlineType.None},
			    new Object[]{&quot;Color&quot;, Color.Black},
			    new Object[]{&quot;IsBold&quot;, false},
			    new Object[]{&quot;IsItalic&quot;, false},
			    new Object[]{&quot;IsStrikeout&quot;, false},
			    new Object[]{&quot;IsSubscript&quot;, false},
                new Object[] {&quot;IsSuperscript&quot;, false}});	         
            //=================Walls====================//
            Walls walls = chart.Walls;
            Console.WriteLine(walls.ForegroundColor);
            Console.WriteLine(walls.BackgroundColor);

        }
```

### See Also

* class [TickLabels](../../ticklabels/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


