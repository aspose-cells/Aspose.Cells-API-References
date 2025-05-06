---
title: Series.XErrorBar
second_title: Aspose.Cells for .NET API Reference
description: Series property. Represents X direction error bar of the series
type: docs
url: /net/aspose.cells.charts/series/xerrorbar/
---
## Series.XErrorBar property

Represents X direction error bar of the series.

```csharp
public ErrorBar XErrorBar { get; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(ErrorBarDisplayType.None, aseries.XErrorBar.DisplayType, &amp;quot;aseries.XErrorBar.DisplayType&amp;quot;);
[Test]
        public void Property_XErrorBar()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Charts\\Scatter.xls&quot;);
            Worksheet worksheet = workbook.Worksheets[0];
            Chart chart = worksheet.Charts[0];
            ReflectInvoker.invoke(&quot;chart&quot;, chart, new Object[][]{
			    new Object[]{&quot;Type&quot;, ChartType.Scatter},
                new Object[] {&quot;IsRectangularCornered&quot;, true},
                new Object[] { &quot;ShowLegend&quot;, true},
               });
            ReflectInvoker.invoke(&quot;chart.ChartObject&quot;, chart.ChartObject, new Object[][]{
                new Object[] { &quot;IsPrintable&quot;, true},
			    new Object[]{&quot;IsLocked&quot;, true},
                new Object[] {&quot;Placement&quot;, PlacementType.Move}});
            //===============ChartArea==================//
            ChartArea chartArea = chart.ChartArea;
            //AssertHelper.assertEquals(&quot;chartArea.getBorder.isAuto&quot;, true, chartArea.getBorder().isAuto());
            AssertHelper.AreEqual(FormattingType.Automatic, chartArea.Area.Formatting, &quot;chartArea.Area.Formatting&quot;);
            ReflectInvoker.invoke(&quot;chartArea&quot;, chartArea, new Object[][]{
			    new Object[]{&quot;Shadow&quot;, false},			
			    new Object[] {&quot;AutoScaleFont&quot;, false},
                new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic}});         
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
            //=================Title===================//
            Title title = chart.Title;
            ReflectInvoker.invoke(&quot;title.Border&quot;, title.Border, new Object[][]{
			    new Object[]{&quot;Style&quot;, LineType.Solid},
			    new Object[]{&quot;Color&quot;, Color.Red},
			    new Object[]{&quot;Weight&quot;,WeightType.HairLine}});
            AssertHelper.AreEqual(FormattingType.None, title.Area.Formatting, &quot;title.Area.Formatting&quot;);
            ReflectInvoker.invoke(&quot;title&quot;, title, new Object[][]{
			    new Object[] {&quot;Text&quot;, &quot;Particulate Levels in Rainfall&quot;},
                new Object[] {&quot;Shadow&quot;, false},
                new Object[] {&quot;AutoScaleFont&quot;, false},
                new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic},
			    new Object[] {&quot;TextHorizontalAlignment&quot;, TextAlignmentType.Right},
			    new Object[] {&quot;TextVerticalAlignment&quot;, TextAlignmentType.Bottom},
			    new Object[] {&quot;TextDirection&quot;, TextDirectionType.LeftToRight},
			    new Object[] { &quot;RotationAngle&quot;, -20}});
            ReflectInvoker.invoke(&quot;title.TextFont&quot;, title.TextFont, new Object[][]{
		        new Object[]{&quot;Name&quot;, &quot;Verdana&quot;},
		        new Object[]{&quot;Size&quot;, 14},
		        new Object[]{&quot;Underline&quot;, FontUnderlineType.None},
		        new Object[]{&quot;Color&quot;, Color.Black},
		        new Object[]{&quot;IsBold&quot;, true},
		        new Object[]{&quot;IsItalic&quot;, false},
		        new Object[]{&quot;IsStrikeout&quot;, false},
		        new Object[]{&quot;IsSubscript&quot;, false},
                new Object[] {&quot;IsSuperscript&quot;, false}
			});           
            //====================Legend===============================//
            Legend legend = chart.Legend;
            //AssertHelper.assertEquals(&quot;legend.getBorder.isAuto&quot;, true, legend.getBorder().isAuto());
            AssertHelper.AreEqual(FormattingType.Automatic, legend.Area.Formatting, &quot;legend.Area.Formatting&quot;);
            ReflectInvoker.invoke(&quot;legend&quot;, legend, new Object[][]{
                new Object[] {&quot;Shadow&quot;, false},
                new Object[] {&quot;AutoScaleFont&quot;, false},
                new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic},
			    new Object[]{&quot;Position&quot;, LegendPositionType.Top}});                 
            ReflectInvoker.invoke(&quot;legend.TextFont&quot;, legend.TextFont, new Object[][]{
			    new Object[]{&quot;Name&quot;, &quot;Tahoma&quot;},
			    new Object[]{&quot;Size&quot;, 10},
			    new Object[]{&quot;Underline&quot;, FontUnderlineType.None},
			    new Object[]{&quot;Color&quot;, Color.Black},
			    new Object[]{&quot;IsBold&quot;, false},
			    new Object[]{&quot;IsItalic&quot;, false},
			    new Object[]{&quot;IsStrikeout&quot;, false},
			    new Object[]{&quot;IsSubscript&quot;, false},
                new Object[] {&quot;IsSuperscript&quot;, false}});
            //======================PlotArea===========================//
            ReflectInvoker.invoke(&quot;chart.PlotArea.Border&quot;, chart.PlotArea.Border, new Object[][]{
			new Object[]{&quot;Style&quot;, LineType.Solid},
			new Object[]{&quot;Color&quot;, Color.Empty},
			new Object[]{&quot;Weight&quot;,WeightType.HairLine}});
            AssertHelper.AreEqual(FormattingType.Automatic, chart.PlotArea.Area.Formatting, &quot;Automatic, chart.PlotArea.Area.Formatting&quot;);
            //=====================NSeries===========================//
            SeriesCollection nseries = chart.NSeries;
            //ReflectInvoker.invoke(&quot;nseries&quot;, nseries, new Object[][]{
            //    new Object[]{&quot;CategoryData&quot;, &quot;=Scatter!$B$2:$B$10&quot;}
            //});
            //====================ASeries===========================//
            Series aseries = nseries[0];
            AssertHelper.AreEqual(false, aseries.Border.IsVisible, &quot;aseries.Line.IsVisible&quot;);
            ReflectInvoker.invoke(&quot;aseries&quot;, aseries, new Object[][]{
				new Object[]{&quot;Name&quot;, &quot;Particulate&quot;},
				new Object[]{&quot;XValues&quot;, &quot;=Scatter!$A$2:$A$10&quot;},
                new Object[]{&quot;Values&quot;, &quot;=Scatter!$B$2:$B$10&quot;},
				new Object[]{&quot;IsColorVaried&quot;, false},
                //new Object[]{&quot;MarkerStyle&quot;, ChartMarkerType.Diamond},
				//new Object[]{&quot;MarkerForegroundColor&quot;, Color.Black},
				//new Object[]{&quot;MarkerBackgroundColor&quot;, Color.Black},
				//new Object[]{&quot;MarkerSize&quot;, 5},
                new Object[] {&quot;Shadow&quot;, false}
			});
            AssertHelper.AreEqual(ChartMarkerType.Diamond, aseries.Marker.MarkerStyle, &quot;aseries.Marker.MarkerStyle&quot;);
            AssertHelper.IsTrue(Util.CompareColor(Color.FromArgb(0x80), aseries.Marker.ForegroundColor), &quot;aseries.Marker.ForegroundColor&quot;);
            AssertHelper.IsTrue(Util.CompareColor(Color.FromArgb(0x80), aseries.Marker.BackgroundColor), &quot;aseries.Marker.BackgroundColor&quot;);
            //AssertHelper.AreEqual(Color.FromArgb(0x80), aseries.Marker.ForegroundColor, &quot;aseries.Marker.ForegroundColor&quot;);
            //AssertHelper.AreEqual(Color.FromArgb(0x80), aseries.Marker.BackgroundColor, &quot;aseries.Marker.BackgroundColor&quot;);
            AssertHelper.AreEqual(5, aseries.Marker.MarkerSize, &quot;aseries.Marker.MarkerSize&quot;);

            AssertHelper.AreEqual(ErrorBarDisplayType.None, aseries.XErrorBar.DisplayType, &quot;aseries.XErrorBar.DisplayType&quot;);
            AssertHelper.AreEqual(ErrorBarDisplayType.None, aseries.YErrorBar.DisplayType, &quot;aseries.YErrorBar.DisplayType&quot;);
            //====================DataLabels=======================//
            DataLabels datalabels = aseries.DataLabels;
            ReflectInvoker.invoke(&quot;datalabels&quot;, datalabels, new Object[][]{
			new Object[]{ &quot;ShowSeriesName&quot;, false},
			new Object[]{ &quot;ShowValue&quot;, false},
			new Object[]{&quot;Separator&quot;, DataLabelsSeparatorType.Auto}});
            //================CategoryAxis========================//
            Axis categoryAxis = chart.CategoryAxis;
           // AssertHelper.assertEquals(&quot;valuexAxis.getAxisLine.isAuto&quot;, true, valuexAxis.getAxisLine().isAuto());
            ReflectInvoker.invoke(&quot;categoryAxis&quot;, categoryAxis, new Object[][]{
				new Object[] {&quot;MajorTickMark&quot;, TickMarkType.Cross},
				new Object[] {&quot;MinorTickMark&quot;, TickMarkType.None},
				new Object[] {&quot;TickLabelPosition&quot;, TickLabelPositionType.NextToAxis},
				new Object[] {&quot;DisplayUnit&quot;, DisplayUnitType.None},
				new Object[] {&quot;IsLogarithmic&quot;, false},
				new Object[] {&quot;IsPlotOrderReversed&quot;, false},
				//new Object[] {&quot;isCrossAtMax&quot;, false},
                new Object[] {&quot;IsVisible&quot;, true}
				});
            AssertHelper.AreEqual(false, categoryAxis.MajorGridLines.IsVisible, &quot;categoryAxis.MajorGridLines.IsVisible&quot;);
            AssertHelper.AreEqual(false, categoryAxis.MinorGridLines.IsVisible, &quot;categoryAxis.MinorGridLines.IsVisible&quot;);
            ReflectInvoker.invoke(&quot;categoryAxis.TickLabels&quot;, categoryAxis.TickLabels, new Object[][]{
				new Object[] {&quot;AutoScaleFont&quot;, false},
                new Object[] { &quot;BackgroundMode&quot;,  BackgroundMode.Automatic},
                new Object[] {&quot;NumberFormatLinked&quot;, true},
                new Object[] {&quot;TextDirection&quot;, TextDirectionType.Context},
                new Object[] { &quot;RotationAngle&quot;, 0}
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
            //==========//
            Title categoryTitle = categoryAxis.Title;
            AssertHelper.AreEqual(false, categoryTitle.Border.IsVisible, &quot;categoryAxis.Title.Border.IsVisible&quot;);
            AssertHelper.AreEqual(FormattingType.None, categoryTitle.Area.Formatting, &quot;categoryAxis.Title.Area.Formatting&quot;);
            ReflectInvoker.invoke(&quot;categoryAxis.Title&quot;, categoryTitle, new Object[][]{
				new Object[] {&quot;Text&quot;, &quot;Daily Rainfall&quot;},
                new Object[] {&quot;Shadow&quot;, false},
                new Object[] {&quot;AutoScaleFont&quot;, false},
                new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic},
				new Object[] {&quot;TextHorizontalAlignment&quot;, TextAlignmentType.Center},
				new Object[] {&quot;TextVerticalAlignment&quot;, TextAlignmentType.Center},
				new Object[] {&quot;TextDirection&quot;, TextDirectionType.Context},
				new Object[] { &quot;RotationAngle&quot;, 0}
			});
            ReflectInvoker.invoke(&quot;categoryAxis.Title.TextFont&quot;, categoryTitle.Font, new Object[][]{
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
            //================ValueAxis========================//
            Axis valueAxis = chart.ValueAxis;
            ReflectInvoker.invoke(&quot;valueAxis.AxisLine&quot;, valueAxis.AxisLine, new Object[][]{
		        new Object[]{&quot;Style&quot;, LineType.Solid},
		        new Object[]{&quot;Color&quot;, Color.Empty},
		        new Object[]{&quot;Weight&quot;,WeightType.HairLine}});
            ReflectInvoker.invoke(&quot;valueAxis&quot;, valueAxis, new Object[][]{
				new Object[] {&quot;MajorTickMark&quot;, TickMarkType.Cross},
				new Object[] {&quot;MinorTickMark&quot;, TickMarkType.None},
				new Object[] {&quot;TickLabelPosition&quot;, TickLabelPositionType.NextToAxis},
				new Object[] {&quot;DisplayUnit&quot;, DisplayUnitType.None},
				new Object[] {&quot;IsLogarithmic&quot;, false},
				new Object[] {&quot;IsPlotOrderReversed&quot;, false},
				//new Object[] {&quot;isCrossAtMax&quot;, false},
                new Object[] {&quot;IsVisible&quot;, true}
				});           
            ReflectInvoker.invoke(&quot;valueAxis.TickLabels&quot;, valueAxis.TickLabels, new Object[][]{
                new Object[] {&quot;AutoScaleFont&quot;, false},
				new Object[] {&quot;NumberFormatLinked&quot;, true},
                new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic},
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
                new Object[] {&quot;IsSuperscript&quot;, false}
			});
            AssertHelper.AreEqual(false, valueAxis.MajorGridLines.IsVisible, &quot;valueAxis.MajorGridLines.IsVisible&quot;);
            AssertHelper.AreEqual(false, valueAxis.MinorGridLines.IsVisible, &quot;valueAxis.MinorGridLines.IsVisible&quot;);
            //==========//
            Title valueAxisTitle = valueAxis.Title;
            AssertHelper.AreEqual(false, valueAxisTitle.Border.IsVisible, &quot;valueAxis.Title.Border.IsVisible&quot;);
            AssertHelper.AreEqual(FormattingType.None, valueAxisTitle.Area.Formatting, &quot;valueAxisTitle.Area.Formatting&quot;);
           
            ReflectInvoker.invoke(&quot;valueAxis.TextFont&quot;, valueAxisTitle.Font, new Object[][]{
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
            ReflectInvoker.invoke(&quot;valueAxis&quot;, valueAxisTitle, new Object[][]{
				new Object[]{&quot;Text&quot;, &quot;Particulate&quot;},
                new Object[] {&quot;Shadow&quot;, false},
                new Object[] {&quot;AutoScaleFont&quot;, false}, 
                new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic},
				new Object[]{&quot;TextHorizontalAlignment&quot;, TextAlignmentType.Center},
				new Object[] {&quot;TextVerticalAlignment&quot;, TextAlignmentType.Center},
				new Object[] {&quot;TextDirection&quot;, TextDirectionType.Context},
				new Object[] { &quot;RotationAngle&quot;, 90}
			});	


        }
```

### See Also

* class [ErrorBar](../../errorbar/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


