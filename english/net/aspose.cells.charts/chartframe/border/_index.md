---
title: ChartFrame.Border
second_title: Aspose.Cells for .NET API Reference
description: ChartFrame property. Gets the border
type: docs
url: /net/aspose.cells.charts/chartframe/border/
---
## ChartFrame.Border property

Gets the [`border`](../../../aspose.cells.drawing/line/).

```csharp
public virtual Line Border { get; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(false, chart.PlotArea.Border.IsVisible, &amp;quot;chart.PlotArea.Border.IsVisible&amp;quot;);
[Test]
        public void Property_Border()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Charts\\FilledRadar.xls&quot;);
            Worksheet worksheet = workbook.Worksheets[0];
            Chart chart = worksheet.Charts[0];
            ReflectInvoker.invoke(&quot;chart&quot;, chart, new Object[][]{
			    new Object[]{&quot;Type&quot;, ChartType.RadarFilled},
                new Object[] {&quot;IsRectangularCornered&quot;, true},              
                new Object[] {&quot;FirstSliceAngle&quot;, 0},
                new Object[] { &quot;ShowLegend&quot;, true}});          
            ReflectInvoker.invoke(&quot;chart.ChartObject&quot;, chart.ChartObject, new Object[][]{
                new Object[] { &quot;IsPrintable&quot;, true},
			    new Object[]{&quot;IsLocked&quot;, true},
                new Object[] {&quot;Placement&quot;, PlacementType.Move}});   
            //============ChartArea===============//
            ChartArea chartArea = chart.ChartArea;
            //AssertHelper.AreEqual(true, chartArea.Border.IsAuto, &quot;chartArea.Border.IsAuto&quot;);
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
				new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic},
			});    
            //=============Title======================//
            Title title = chart.Title;
            AssertHelper.AreEqual(false, title.Border.IsVisible, &quot;title.Border.IsVisible&quot;);
            AssertHelper.AreEqual(FormattingType.None, title.Area.Formatting, &quot;title.Area.Formatting&quot;);
            ReflectInvoker.invoke(&quot;title&quot;, title, new Object[][]{
                  new Object[] {&quot;Text&quot;, &quot;Nutritional Analysis&quot;},
                  new Object[] {&quot;Shadow&quot;, false},
			      new Object[]{&quot;AutoScaleFont&quot;, false},
			      new Object[]{ &quot;BackgroundMode&quot;, BackgroundMode.Automatic},
                  new Object[] {&quot;TextHorizontalAlignment&quot;, TextAlignmentType.Center},
                  new Object[] {&quot;TextVerticalAlignment&quot;, TextAlignmentType.Center},
                  new Object[] {&quot;TextDirection&quot;, TextDirectionType.Context},
                  new Object[] { &quot;RotationAngle&quot;, 0}
			});         
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
            //=============Legend=====================//
            Legend legend = chart.Legend;
            //AssertHelper.AreEqual(true, legend.Border.IsAuto, &quot;legend.Border.IsAuto&quot;);
            AssertHelper.AreEqual(FormattingType.Automatic, legend.Area.Formatting, &quot;legend.Area.Formatting&quot;);
            ReflectInvoker.invoke(&quot;legend&quot;, legend, new Object[][]{
                new Object[] {&quot;Shadow&quot;, false},
                new Object[] {&quot;AutoScaleFont&quot;, false},
                new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic},
                new Object[] {&quot;Position&quot;, LegendPositionType.Right}
              });
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
            //==========PlotArea=================//
            AssertHelper.AreEqual(false, chart.PlotArea.Border.IsVisible, &quot;chart.PlotArea.Border.IsVisible&quot;);
            AssertHelper.AreEqual(FormattingType.Automatic, chart.PlotArea.Area.Formatting, &quot;chart.PlotArea.Area.Formatting&quot;);
            //=================NSeries==========================//
            SeriesCollection nseries = chart.NSeries;
            ReflectInvoker.invoke(&quot;nseries&quot;, nseries, new Object[][]{
				new Object[]{&quot;CategoryData&quot;, &quot;=Sheet1!$B$1:$G$1&quot;},
				new Object[]{&quot;Count&quot;, 3}
			});
            //===================ASeries=====================//
            Series aseries = nseries[0];
            ReflectInvoker.invoke(&quot;aseries&quot;, aseries, new Object[][]{
				new Object[]{&quot;Name&quot;, &quot;Brand A&quot;},
				new Object[]{&quot;Values&quot;, &quot;=Sheet1!$B$2:$G$2&quot;},
				new Object[]{&quot;PlotOnSecondAxis&quot;, false}
			});
            //AssertHelper.assertEquals(&quot;aseries.getBorder.isAuto&quot;, true, aseries.getBorder().isAuto());
            AssertHelper.AreEqual(FormattingType.Automatic, aseries.Area.Formatting, &quot;aseries.Area.Formatting&quot;);
            //===================DataLabels=====================//
            DataLabels datalabels = aseries.DataLabels;
            ReflectInvoker.invoke(&quot;datalabels&quot;, datalabels, new Object[][]{
				new Object[]{ &quot;ShowSeriesName&quot;, false},
				new Object[]{ &quot;ShowCategoryName&quot;, false},
				new Object[]{ &quot;ShowValue&quot;, false},
				new Object[]{ &quot;SeparatorType&quot;, DataLabelsSeparatorType.Auto},		
			});	
            //===========valueAxis=======================//
            Axis valueAxis = chart.ValueAxis;
            ReflectInvoker.invoke(&quot;valueAxis.AxisLine&quot;, valueAxis.AxisLine, new Object[][]{
			    new Object[] {&quot;Style&quot;, LineType.Solid},
                new Object[] {&quot;Color&quot;, Color.Empty},
                new Object[] {&quot;Weight&quot;, WeightType.HairLine}
              });
            ReflectInvoker.invoke(&quot;valueAxis&quot;, valueAxis, new Object[][]{
			    new Object[] {&quot;MinorTickMark&quot;, TickMarkType.None},
                new Object[] {&quot;TickLabelPosition&quot;, TickLabelPositionType.NextToAxis},
                new Object[] {&quot;DisplayUnit&quot;, DisplayUnitType.None},
                new Object[] {&quot;IsLogarithmic&quot;, false},
                new Object[] {&quot;IsVisible&quot;, true}
            });
            AssertHelper.AreEqual(true, valueAxis.MajorGridLines.IsVisible, &quot;valueAxis.MajorGridLines.IsVisible&quot;);
            AssertHelper.AreEqual(false, valueAxis.MinorGridLines.IsVisible, &quot;valueAxis.MinorGridLines.IsVisible&quot;);
            ReflectInvoker.invoke(&quot;valueAxis.TickLabels&quot;, valueAxis.TickLabels, new Object[][]{
                new Object[] {&quot;AutoScaleFont&quot;, false},
                new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic},
			    new Object[] {&quot;NumberFormatLinked&quot;, true},
                new Object[] { &quot;RotationAngle&quot;, 0},
                new Object[] {&quot;TextDirection&quot;, TextDirectionType.Context}                
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
            //====================CategoryAxis=======================//
            Axis categoryAxis = chart.CategoryAxis;
            TickLabels ticklabels = categoryAxis.TickLabels;
            ReflectInvoker.invoke(&quot;categoryAxis.TickLabels.Font&quot;, ticklabels.Font, new Object[][]{
			    new Object[]{&quot;Name&quot;, &quot;Tahoma&quot;},
			    new Object[]{&quot;Size&quot;, 10},
			    new Object[]{&quot;Underline&quot;, FontUnderlineType.None},
			    new Object[]{&quot;Color&quot;, Color.Black},
			    new Object[]{&quot;IsBold&quot;, false},
			    new Object[]{&quot;IsItalic&quot;, false},
			    new Object[]{&quot;IsStrikeout&quot;, false},
			    new Object[]{&quot;IsSubscript&quot;, false},
                new Object[] {&quot;IsSuperscript&quot;, false}});
            ReflectInvoker.invoke(&quot;categoryAxis.Title&quot;, ticklabels, new Object[][]{
                new Object[] {&quot;AutoScaleFont&quot;, false},
                new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic},
			    new Object[] { &quot;RotationAngle&quot;, 30},
			    new Object[] {&quot;TextDirection&quot;, TextDirectionType.Context}});  
        }
```

### See Also

* class [Line](../../../aspose.cells.drawing/line/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


