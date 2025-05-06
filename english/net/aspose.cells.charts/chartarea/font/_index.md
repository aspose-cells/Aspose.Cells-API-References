---
title: ChartArea.Font
second_title: Aspose.Cells for .NET API Reference
description: ChartArea property. Gets a Font object of the specified chartarea object
type: docs
url: /net/aspose.cells.charts/chartarea/font/
---
## ChartArea.Font property

Gets a `Font` object of the specified chartarea object.

```csharp
public override Font Font { get; }
```

### Examples

```csharp
// Called: ReflectInvoker.invoke(&amp;quot;chartArea.TextFont&amp;quot;, chartArea.Font, new Object[][]{
[Test]
        public void Property_Font()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Charts\\StackedLine.xls&quot;);
            Worksheet worksheet = workbook.Worksheets[0];
            Chart chart = worksheet.Charts[0];
            ReflectInvoker.invoke(&quot;chart&quot;, chart, new Object[][]{
			    new Object[]{&quot;Type&quot;, ChartType.LineStackedWithDataMarkers},
                new Object[] {&quot;IsRectangularCornered&quot;, false},
                new Object[] { &quot;ShowLegend&quot;, true},
                new Object[] { &quot;ShowDataTable&quot;, false}
               });
            ReflectInvoker.invoke(&quot;chart.ChartObject&quot;, chart.ChartObject, new Object[][]{
                new Object[] { &quot;IsPrintable&quot;, true},
			    new Object[]{&quot;IsLocked&quot;, true},
                new Object[] {&quot;Placement&quot;, PlacementType.Move}});
            //===================ChartArea=========================//
            ChartArea chartArea = chart.ChartArea;
            //AssertHelper.assertEquals(&quot;chartArea.getBorder.isAuto&quot;, true, chartArea.getBorder().isAuto());
            AssertHelper.AreEqual(FormattingType.Automatic, chartArea.Area.Formatting, &quot;chartArea.Area.Formatting&quot;);         
            ReflectInvoker.invoke(&quot;chartArea.TextFont&quot;, chartArea.Font, new Object[][]{
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
            ReflectInvoker.invoke(&quot;chartArea&quot;, chartArea, new Object[][]{
			    new Object[]{&quot;Shadow&quot;, false},
			    new Object[]{&quot;AutoScaleFont&quot;, false},
			    new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic}});          
            //=================Title===================//
            Title title = chart.Title;
            AssertHelper.AreEqual(false, title.Border.IsVisible, &quot;title.Border.IsVisible&quot;);
            AssertHelper.AreEqual(FormattingType.None, title.Area.Formatting, &quot;title.Area.Formatting&quot;);
            ReflectInvoker.invoke(&quot;title&quot;, title, new Object[][]{
			    new Object[] {&quot;Text&quot;, &quot;Sales By Region For Years&quot;},
                new Object[] {&quot;Shadow&quot;, false},
                new Object[] {&quot;AutoScaleFont&quot;, false},
                new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic},
			    new Object[] {&quot;TextHorizontalAlignment&quot;, TextAlignmentType.Center},
			    new Object[] {&quot;TextVerticalAlignment&quot;, TextAlignmentType.Center},
			    new Object[] {&quot;TextDirection&quot;, TextDirectionType.Context},
			    new Object[] { &quot;RotationAngle&quot;, 0}});

            ReflectInvoker.invoke(&quot;title.TextFont&quot;, title.Font, new Object[][]{
			    new Object[]{&quot;Name&quot;, &quot;Arial&quot;},
			    new Object[]{&quot;Size&quot;, 12},
			    new Object[]{&quot;Underline&quot;, FontUnderlineType.None},
			    new Object[]{&quot;Color&quot;, Color.Black},
			    new Object[]{&quot;IsBold&quot;, true},
			    new Object[]{&quot;IsItalic&quot;, false},
			    new Object[]{&quot;IsStrikeout&quot;, false},
			    new Object[]{&quot;IsSubscript&quot;, false},
                new Object[] {&quot;IsSuperscript&quot;, false}
			}); 
            //=================Legend====================//
            Legend legend = chart.Legend;
            //AssertHelper.assertEquals(&quot;legend.getBorder.isAuto&quot;, true, legend.getBorder().isAuto());
            AssertHelper.AreEqual(FormattingType.Automatic, legend.Area.Formatting, &quot;legend.Area.Formatting&quot;);         
            ReflectInvoker.invoke(&quot;legend.TextFont&quot;, legend.Font, new Object[][]{
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
            ReflectInvoker.invoke(&quot;legend&quot;, legend, new Object[][]{
			    new Object[] {&quot;Shadow&quot;, false},
                new Object[] {&quot;AutoScaleFont&quot;, false},
                new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic},
                new Object[] {&quot;Position&quot;, LegendPositionType.Top}
             });
            //=================PlotArea=====================// 
            ReflectInvoker.invoke(&quot;chart.PlotArea.Border&quot;, chart.PlotArea.Border, new Object[][]{
				new Object[]{&quot;Style&quot;, LineType.Solid},
				new Object[]{&quot;Color&quot;, Color.Empty},
				new Object[]{&quot;Weight&quot;,WeightType.HairLine}});
            AssertHelper.AreEqual(FormattingType.Automatic, chart.PlotArea.Area.Formatting, &quot;chart.PlotArea.Area.Formatting&quot;);
            //==================NSeries=====================//
            SeriesCollection nseries = chart.NSeries;
            ReflectInvoker.invoke(&quot;nseries&quot;, nseries, new Object[][]{
			new Object[]{&quot;CategoryData&quot;, &quot;=Sheet1!$B$1:$F$1&quot;},
			new Object[]{&quot;Count&quot;, 3}});
            //===================ASeries=====================//
            Series aseries = nseries[0];
            // AssertHelper.assertEquals(&quot;aseries.getBorder.isAuto&quot;, true, aseries.getBorder().isAuto());
            AssertHelper.AreEqual(FormattingType.Automatic, aseries.Area.Formatting, &quot;aseries.Area.Formatting&quot;);
            ReflectInvoker.invoke(&quot;aseries&quot;, aseries, new Object[][]{
				new Object[] {&quot;Name&quot;, &quot;France&quot;},
				new Object[] {&quot;Values&quot;, &quot;=Sheet1!$B$2:$F$2&quot;},
				//new Object[] {&quot;MarkerSize&quot;, 5},
                new Object[] {&quot;Shadow&quot;, false},
				new Object[] {&quot;GapWidth&quot;, (short)150},
				new Object[] {&quot;HasDropLines&quot;, true},
				new Object[] {&quot;HasHiLoLines&quot;, true},
				new Object[] {&quot;HasUpDownBars&quot;, true}
			});
            AssertHelper.AreEqual(5, aseries.Marker.MarkerSize, &quot;aseries.Marker.MarkerSize&quot;);
            AssertHelper.AreEqual(ErrorBarDisplayType.None, aseries.YErrorBar.DisplayType, &quot;aseries.YErrorBar.DisplayType&quot;);
            //==================DataLabels======================//
            DataLabels datalabels = aseries.DataLabels;
            ReflectInvoker.invoke(&quot;datalabels&quot;, datalabels, new Object[][]{
			new Object[]{ &quot;ShowSeriesName&quot;, false},
			new Object[]{ &quot;ShowCategoryName&quot;, false},
			new Object[]{ &quot;ShowValue&quot;, false},
			new Object[]{&quot;SeparatorType&quot;, DataLabelsSeparatorType.Auto}});
            //=================CategoryAxis====================//
            Axis categoryAxis = chart.CategoryAxis;
            AssertHelper.AreEqual(false, categoryAxis.MajorGridLines.IsVisible, &quot;categoryAxis.MajorGridLines.IsVisible&quot;);
            AssertHelper.AreEqual(false, categoryAxis.MinorGridLines.IsVisible, &quot;categoryAxis.MinorGridLines.IsVisible&quot;);

            ReflectInvoker.invoke(&quot;categoryAxis.AxisLine&quot;, categoryAxis.AxisLine, new Object[][]{
			    new Object[]{&quot;Style&quot;, LineType.Solid},
			    new Object[]{&quot;Color&quot;, Color.Empty},
			    new Object[]{&quot;Weight&quot;, WeightType.HairLine}});      
            ReflectInvoker.invoke(&quot;categoryAxis&quot;, categoryAxis, new Object[][]{
				new Object[] {&quot;MajorTickMark&quot;, TickMarkType.Cross},
				new Object[] {&quot;MinorTickMark&quot;, TickMarkType.None},
				new Object[] {&quot;TickLabelPosition&quot;, TickLabelPositionType.NextToAxis},
				new Object[] {&quot;TickLabelSpacing&quot;, 1},
				new Object[] {&quot;TickMarkSpacing&quot;, 1},
				new Object[] {&quot;AxisBetweenCategories&quot;, true},
				new Object[] {&quot;IsPlotOrderReversed&quot;, false},
				//new Object[] {&quot;isCrossAtMax&quot;, false},			
	            new Object[] {&quot;IsVisible&quot;, true}
		   });
            ReflectInvoker.invoke(&quot;categoryAxis.TickLabels&quot;, categoryAxis.TickLabels, new Object[][]{
			    new Object[]{&quot;AutoScaleFont&quot;, false},
                new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic},
                new Object[] {&quot;NumberFormatLinked&quot;, true},
                new Object[] { &quot;RotationAngle&quot;, 0},
                new Object[] {&quot;Offset&quot;, 100},
                new Object[] {&quot;TextDirection&quot;, TextDirectionType.Context}
            });
            ReflectInvoker.invoke(&quot;categoryAxis.TickLabels.Font&quot;, categoryAxis.TickLabels.Font, new Object[][]{
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
            //==================CategoryAxis.getTitle===========//
            Title categoryTilte = categoryAxis.Title;
            ReflectInvoker.invoke(&quot;categoryAxis.Title&quot;, categoryTilte, new Object[][]{
				new Object[]{&quot;Text&quot;, &quot;Year(2002-2006)&quot;},
                new Object[]{&quot;Shadow&quot;, false},
                new Object[]{&quot;AutoScaleFont&quot;, false},
                new Object[]{ &quot;BackgroundMode&quot;, BackgroundMode.Automatic},
				new Object[]{&quot;TextHorizontalAlignment&quot;, TextAlignmentType.Center},
				new Object[]{&quot;TextVerticalAlignment&quot;, TextAlignmentType.Center},
				new Object[]{&quot;TextDirection&quot;, TextDirectionType.Context},
				new Object[]{ &quot;RotationAngle&quot;, 0}});

            AssertHelper.AreEqual(false, categoryTilte.Border.IsVisible, &quot;categoryAxis.Title.Border.IsVisible&quot;);
            AssertHelper.AreEqual(FormattingType.None, categoryTilte.Area.Formatting, &quot;categoryTilte.Area.Formatting&quot;);          
            ReflectInvoker.invoke(&quot;categoryAxis.getTitle.TextFont&quot;, categoryTilte.Font, new Object[][]{
			    new Object[]{&quot;Name&quot;, &quot;Arial&quot;},
			    new Object[]{&quot;Size&quot;, 10},
			    new Object[]{&quot;Underline&quot;, FontUnderlineType.None},
			    new Object[]{&quot;Color&quot;, Color.Black},
			    new Object[]{&quot;IsBold&quot;, true},
			    new Object[]{&quot;IsItalic&quot;, false},
			    new Object[]{&quot;IsStrikeout&quot;, false},
			    new Object[]{&quot;IsSubscript&quot;, false},
                new Object[] {&quot;IsSuperscript&quot;, false}
			});
            //=====================ValueAxis=========================//
            Axis valueAxis = chart.ValueAxis;
            AssertHelper.AreEqual(false, valueAxis.MajorGridLines.IsVisible, &quot;valueAxis.MajorGridLines.IsVisible&quot;);
            AssertHelper.AreEqual(false, valueAxis.MinorGridLines.IsVisible, &quot;valueAxis.MinorGridLines.IsVisible&quot;);

            ReflectInvoker.invoke(&quot;valueAxis.AxisLine&quot;, valueAxis.AxisLine, new Object[][]{
			    new Object[]{&quot;Style&quot;, LineType.Solid},
			    new Object[]{&quot;Color&quot;, Color.Empty},
			    new Object[]{&quot;Weight&quot;, WeightType.HairLine}});
            ReflectInvoker.invoke(&quot;valueAxis&quot;, valueAxis, new Object[][]{
				new Object[] {&quot;MajorTickMark&quot;, TickMarkType.Outside},
				new Object[] {&quot;MinorTickMark&quot;, TickMarkType.Cross},
				new Object[] {&quot;TickLabelPosition&quot;, TickLabelPositionType.High},
				//new Object[] {&quot;isAutoCross&quot;, true},
				new Object[] {&quot;DisplayUnit&quot;, DisplayUnitType.Hundreds},
				//new Object[] {&quot;isDisplayUnitLabelShown&quot;, false},
				new Object[] {&quot;IsLogarithmic&quot;, false},
				new Object[] {&quot;IsPlotOrderReversed&quot;, false},
				//new Object[] {&quot;isCrossAtMax&quot;, false},
                new Object[] {&quot;IsVisible&quot;, true}
		   });
            ReflectInvoker.invoke(&quot;valueAxis.TickLabels&quot;, valueAxis.TickLabels, new Object[][]{
			    new Object[]{&quot;AutoScaleFont&quot;, false},
                new Object[]{ &quot;BackgroundMode&quot;, BackgroundMode.Automatic}
               });
            ReflectInvoker.invoke(&quot;valueAxis.TickLabels.Font&quot;, valueAxis.TickLabels.Font, new Object[][]{
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

        }
```

### See Also

* class [Font](../../../aspose.cells/font/)
* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


