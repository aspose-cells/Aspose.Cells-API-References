---
title: ErrorBar.DisplayType
second_title: Aspose.Cells for .NET API Reference
description: ErrorBar property. Represents the display type of error bar
type: docs
url: /net/aspose.cells.charts/errorbar/displaytype/
---
## ErrorBar.DisplayType property

Represents the display type of error bar.

```csharp
public ErrorBarDisplayType DisplayType { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(ErrorBarDisplayType.None, aseries.YErrorBar.DisplayType, &amp;quot;aseries.YErrorBar.DisplayType&amp;quot;);
[Test]
        public void Property_DisplayType()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Charts\\Bubble.xls&quot;);
            Worksheet worksheet = workbook.Worksheets[0];
            Chart chart = worksheet.Charts[0];

            ReflectInvoker.invoke(&quot;chart&quot;, chart, new Object[][]{
			new Object[]{&quot;Type&quot;, ChartType.Bubble},
            new Object[] {&quot;IsRectangularCornered&quot;, false},
            new Object[] { &quot;ShowLegend&quot;, true}});
            Console.WriteLine(&quot;Chart&quot;);
            //===============ChartArea==================//
            ChartArea chartArea = chart.ChartArea;
            ReflectInvoker.invoke(&quot;chartArea&quot;, chartArea, new Object[][]{
			    new Object[]{&quot;Shadow&quot;, false},
                new Object[] {&quot;AutoScaleFont&quot;, true},
                new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic}
		    });
            Console.WriteLine(&quot;ChartArea&quot;);
            AssertHelper.AreEqual(FormattingType.Automatic, chartArea.Area.Formatting, &quot;chartArea.Area.Formatting&quot;);

            ReflectInvoker.invoke(&quot;chartArea.getFont&quot;, chartArea.TextFont, new Object[][]{
			    new Object[] {&quot;Name&quot;, FontNameConstants.zh_SongTi},
			    new Object[] {&quot;Size&quot;, 12},
			    new Object[] {&quot;Underline&quot;, FontUnderlineType.None},			 
			    new Object[] {&quot;IsBold&quot;, false},
			    new Object[] {&quot;IsItalic&quot;, false},
			    new Object[] {&quot;IsStrikeout&quot;, false},
                new Object[] {&quot;IsSubscript&quot;, false},
                new Object[] {&quot;IsSuperscript&quot;, false}
			    });
            Console.WriteLine(&quot;ChartArea.font&quot;);
            AssertHelper.equals(Color.Black, chartArea.TextFont.Color, &quot;chartArea.getFont.Color&quot;);
            ReflectInvoker.invoke(&quot;chart.ChartObject&quot;, chart.ChartObject, new Object[][]{
			    new Object[]{ &quot;IsPrintable&quot;, true},
			    new Object[]{&quot;IsLocked&quot;, true},
			    new Object[] {&quot;Placement&quot;, PlacementType.MoveAndSize}
		    });
            Console.WriteLine(&quot;ChartObject&quot;);
            //=====================Title========================//
            Title title = chart.Title;
            ReflectInvoker.invoke(&quot;title&quot;, title, new Object[][]{
			    new Object[]{&quot;Shadow&quot;, false},
                new Object[] {&quot;AutoScaleFont&quot;, true},
                new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic}
		    });
            Console.WriteLine(&quot;title&quot;);
            AssertHelper.AreEqual(false, title.Border.IsVisible, &quot;title.Border.IsVisible&quot;);
            AssertHelper.AreEqual(FormattingType.None, title.Area.Formatting, &quot;title.Area.Formatting&quot;);
            ReflectInvoker.invoke(&quot;title.getFont&quot;, title.TextFont, new Object[][]{
			    new Object[]{&quot;Name&quot;, FontNameConstants.zh_SongTi},
			    new Object[]{&quot;Size&quot;, 12},
			    new Object[]{&quot;Underline&quot;, FontUnderlineType.None},
			    new Object[]{&quot;IsBold&quot;, false},
			    new Object[]{&quot;IsItalic&quot;, false},
			    new Object[]{&quot;IsStrikeout&quot;, false},
			    new Object[]{&quot;IsSubscript&quot;, false},
                new Object[] {&quot;IsSuperscript&quot;, false}
			});
            Console.WriteLine(&quot;title.font&quot;);
            AssertHelper.equals(Color.Black, title.TextFont.Color, &quot;title.TextFont.Color&quot;);
            ReflectInvoker.invoke(&quot;title&quot;, title, new Object[][]{
                new Object[] {&quot;Shadow&quot;, false},
				new Object[]{&quot;Text&quot;, &quot;Industry Market Share Study&quot;},
				new Object[]{&quot;TextHorizontalAlignment&quot;, TextAlignmentType.Center},
				new Object[]{&quot;TextVerticalAlignment&quot;, TextAlignmentType.Center},
				new Object[]{&quot;TextDirection&quot;, TextDirectionType.Context},
				new Object[]{ &quot;RotationAngle&quot;, 0}
			});
            Console.WriteLine(&quot;title.option&quot;);
            //================Legend=======================//
            Legend legend = chart.Legend;         
            AssertHelper.AreEqual(FormattingType.Automatic, legend.Area.Formatting, &quot;legend.Area.Formatting&quot;);
            ReflectInvoker.invoke(&quot;legend&quot;, legend, new Object[][]{
			    new Object[]{&quot;Shadow&quot;, false},
                new Object[] {&quot;AutoScaleFont&quot;, true},
                new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic}
		    });
            Console.WriteLine(&quot;Legend&quot;);
            ReflectInvoker.invoke(&quot;legend.TextFont&quot;, legend.TextFont, new Object[][]{
			    new Object[]{&quot;Name&quot;, FontNameConstants.zh_SongTi},
			    new Object[]{&quot;Size&quot;, 12},
			    new Object[]{&quot;Underline&quot;, FontUnderlineType.None},
			    new Object[]{&quot;IsBold&quot;, false},
			    new Object[]{&quot;IsItalic&quot;, false},
			    new Object[]{&quot;IsStrikeout&quot;, false},
			    new Object[]{&quot;IsSubscript&quot;, false},
                new Object[]{&quot;IsSuperscript&quot;, false}
			});
            Console.WriteLine(&quot;Legend.font&quot;);
            AssertHelper.equals(Color.Black, legend.TextFont.Color, &quot;legend.TextFont.Color&quot;);
            //=================ASeries=======================//
            SeriesCollection nseries = chart.NSeries;
            Series aseries = nseries[0];
            AssertHelper.AreEqual(FormattingType.Automatic, aseries.Area.Formatting, &quot;FormattingType.Automatic&quot;);
            ReflectInvoker.invoke(&quot;aseries&quot;, aseries, new Object[][]{
			    new Object[]{&quot;BubbleSizes&quot;, &quot;=Sheet1!$C$2:$C$4&quot;},
			    new Object[]{&quot;Values&quot;, &quot;=Sheet1!$B$2:$B$4&quot;},
			    new Object[]{&quot;XValues&quot;, &quot;=Sheet1!$A$2:$A$4&quot;},
			    new Object[]{&quot;Name&quot;, &quot;=Sheet1!$B$1&quot;},		
                new Object[] {&quot;SizeRepresents&quot;, BubbleSizeRepresents.SizeIsArea},
                new Object[]{&quot;ShowNegativeBubbles&quot;, true},
			    new Object[]{&quot;IsColorVaried&quot;, true},
                new Object[]{&quot;BubbleScale&quot;, 100}});
            Console.WriteLine(&quot;value&quot;);
            AssertHelper.AreEqual(ErrorBarDisplayType.None, aseries.XErrorBar.DisplayType, &quot;aseries.XErrorBar.DisplayType&quot;);
            AssertHelper.AreEqual(ErrorBarDisplayType.None, aseries.YErrorBar.DisplayType, &quot;aseries.YErrorBar.DisplayType&quot;);
            //====================DataLabels=======================//
            DataLabels datalabels = aseries.DataLabels;
            ReflectInvoker.invoke(&quot;datalabels&quot;, datalabels, new Object[][]{
			    new Object[]{&quot;ShowSeriesName&quot;, false},
			    new Object[]{ &quot;ShowValue&quot;, false},
			    new Object[]{&quot;IsBubbleSizeShown&quot;, false},
			    new Object[]{&quot;Separator&quot;,  DataLabelsSeparatorType.Auto}	});
            Console.WriteLine(&quot;datalabels&quot;);
            //====================CategoryAxis========================//
            Axis categoryaxis = chart.CategoryAxis;
            AssertHelper.AreEqual(false, categoryaxis.MajorGridLines.IsVisible, &quot;categoryaxis.MajorGridLines.IsVisible&quot;);
            AssertHelper.AreEqual(false, categoryaxis.MinorGridLines.IsVisible, &quot;categoryaxis.MinorGridLines.IsVisible&quot;);
            ReflectInvoker.invoke(&quot;categoryaxis&quot;, categoryaxis, new Object[][]{
				new Object[] {&quot;MajorTickMark&quot;, TickMarkType.Cross},
				new Object[] {&quot;MinorTickMark&quot;, TickMarkType.None},
				new Object[] {&quot;TickLabelPosition&quot;, TickLabelPositionType.NextToAxis},				
				new Object[] {&quot;DisplayUnit&quot;, DisplayUnitType.None},
				new Object[] {&quot;IsLogarithmic&quot;, false},
				new Object[] {&quot;IsPlotOrderReversed&quot;, false},
                new Object[] {&quot;IsVisible&quot;, true}
				});
            Console.WriteLine(&quot;categoryaxis&quot;);
            ReflectInvoker.invoke(&quot;categoryaxis.TickLabels.Font&quot;, categoryaxis.TickLabels.Font, new Object[][]{
			    new Object[]{&quot;Name&quot;, FontNameConstants.zh_SongTi},
			    new Object[]{&quot;Size&quot;, 12},
			    new Object[]{&quot;Underline&quot;, FontUnderlineType.None},
			    new Object[]{&quot;IsBold&quot;, false},
			    new Object[]{&quot;IsItalic&quot;, false},
			    new Object[]{&quot;IsStrikeout&quot;, false},
			    new Object[]{&quot;IsSubscript&quot;, false},
                new Object[] {&quot;IsSuperscript&quot;, false}
			});
            Console.WriteLine(&quot;categoryaxis.tickfont&quot;);
            AssertHelper.equals(Color.Black, categoryaxis.TickLabels.Font.Color, &quot;categoryaxis.TickLabels.Font.Color&quot;);
            Console.WriteLine(&quot;categoryaxis.tickfont1&quot;);
            ReflectInvoker.invoke(&quot;categoryaxis.TickLabels&quot;, categoryaxis.TickLabels, new Object[][]{
			    new Object[] {&quot;AutoScaleFont&quot;, true},
                new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic},
                new Object[] {&quot;NumberFormatLinked&quot;, true},
                new Object[] {&quot;TextDirection&quot;, TextDirectionType.Context},
                new Object[] { &quot;RotationAngle&quot;, 0}
            });
            Console.WriteLine(&quot;categoryaxis.tick&quot;);
            //====================ValueAxis========================//
            Axis valueAxis = chart.ValueAxis;
            AssertHelper.AreEqual(true, valueAxis.MajorGridLines.IsVisible, &quot;valueAxis.MajorGridLines.IsVisible&quot;);
            AssertHelper.AreEqual(false, valueAxis.MinorGridLines.IsVisible, &quot;valueAxis.MinorGridLines.IsVisible&quot;);
            Console.WriteLine(&quot;categoryaxis.tick&quot;);
            ReflectInvoker.invoke(&quot;valueAxis&quot;, valueAxis, new Object[][]{
				new Object[] {&quot;MajorTickMark&quot;, TickMarkType.Cross},
				new Object[] {&quot;MinorTickMark&quot;, TickMarkType.None},
				new Object[] {&quot;TickLabelPosition&quot;, TickLabelPositionType.NextToAxis},
				new Object[] {&quot;DisplayUnit&quot;, DisplayUnitType.None},
				new Object[] {&quot;IsLogarithmic&quot;, false},
				new Object[] {&quot;IsPlotOrderReversed&quot;, false},
                new Object[] {&quot;IsVisible&quot;, true}
            });
            ReflectInvoker.invoke(&quot;valueAxis.TickLabels.Font&quot;, valueAxis.TickLabels.Font, new Object[][]{
			    new Object[]{&quot;Name&quot;, FontNameConstants.zh_SongTi},
			    new Object[]{&quot;Size&quot;, 12},
			    new Object[]{&quot;Underline&quot;, FontUnderlineType.None},
			    new Object[]{&quot;IsBold&quot;, false},
			    new Object[]{&quot;IsItalic&quot;, false},
			    new Object[]{&quot;IsStrikeout&quot;, false},
			    new Object[]{&quot;IsSubscript&quot;, false},
                new Object[]{&quot;IsSuperscript&quot;, false}
			});
            AssertHelper.equals(Color.Black, valueAxis.TickLabels.Font.Color, &quot;valueAxis.TickLabels.Font.Color&quot;);

            ReflectInvoker.invoke(&quot; valueAxis.TickLabels&quot;, valueAxis.TickLabels, new Object[][]{
				new Object[] {&quot;AutoScaleFont&quot;, true},
                new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic},
                new Object[] {&quot;NumberFormatLinked&quot;, true},
                new Object[] {&quot;TextDirection&quot;, TextDirectionType.Context},
                new Object[] { &quot;RotationAngle&quot;, 0}
            });
        }
```

### See Also

* enum [ErrorBarDisplayType](../../errorbardisplaytype/)
* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


