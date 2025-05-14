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
// Called: AssertHelper.AreEqual(ErrorBarDisplayType.None, aseries.XErrorBar.DisplayType, "aseries.XErrorBar.DisplayType");
        public void Series_Property_XErrorBar()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "Charts\\Bubble.xls");
            Worksheet worksheet = workbook.Worksheets[0];
            Chart chart = worksheet.Charts[0];

            ReflectInvoker.invoke("chart", chart, new Object[][]{
			new Object[]{"Type", ChartType.Bubble},
            new Object[] {"IsRectangularCornered", false},
            new Object[] { "ShowLegend", true}});
            Console.WriteLine("Chart");
            //===============ChartArea==================//
            ChartArea chartArea = chart.ChartArea;
            ReflectInvoker.invoke("chartArea", chartArea, new Object[][]{
			    new Object[]{"Shadow", false},
                new Object[] {"AutoScaleFont", true},
                new Object[] { "BackgroundMode", BackgroundMode.Automatic}
		    });
            Console.WriteLine("ChartArea");
            AssertHelper.AreEqual(FormattingType.Automatic, chartArea.Area.Formatting, "chartArea.Area.Formatting");

            ReflectInvoker.invoke("chartArea.getFont", chartArea.TextFont, new Object[][]{
			    new Object[] {"Name", FontNameConstants.zh_SongTi},
			    new Object[] {"Size", 12},
			    new Object[] {"Underline", FontUnderlineType.None},			 
			    new Object[] {"IsBold", false},
			    new Object[] {"IsItalic", false},
			    new Object[] {"IsStrikeout", false},
                new Object[] {"IsSubscript", false},
                new Object[] {"IsSuperscript", false}
			    });
            Console.WriteLine("ChartArea.font");
            AssertHelper.equals(Color.Black, chartArea.TextFont.Color, "chartArea.getFont.Color");
            ReflectInvoker.invoke("chart.ChartObject", chart.ChartObject, new Object[][]{
			    new Object[]{ "IsPrintable", true},
			    new Object[]{"IsLocked", true},
			    new Object[] {"Placement", PlacementType.MoveAndSize}
		    });
            Console.WriteLine("ChartObject");
            //=====================Title========================//
            Title title = chart.Title;
            ReflectInvoker.invoke("title", title, new Object[][]{
			    new Object[]{"Shadow", false},
                new Object[] {"AutoScaleFont", true},
                new Object[] { "BackgroundMode", BackgroundMode.Automatic}
		    });
            Console.WriteLine("title");
            AssertHelper.AreEqual(false, title.Border.IsVisible, "title.Border.IsVisible");
            AssertHelper.AreEqual(FormattingType.None, title.Area.Formatting, "title.Area.Formatting");
            ReflectInvoker.invoke("title.getFont", title.TextFont, new Object[][]{
			    new Object[]{"Name", FontNameConstants.zh_SongTi},
			    new Object[]{"Size", 12},
			    new Object[]{"Underline", FontUnderlineType.None},
			    new Object[]{"IsBold", false},
			    new Object[]{"IsItalic", false},
			    new Object[]{"IsStrikeout", false},
			    new Object[]{"IsSubscript", false},
                new Object[] {"IsSuperscript", false}
			});
            Console.WriteLine("title.font");
            AssertHelper.equals(Color.Black, title.TextFont.Color, "title.TextFont.Color");
            ReflectInvoker.invoke("title", title, new Object[][]{
                new Object[] {"Shadow", false},
				new Object[]{"Text", "Industry Market Share Study"},
				new Object[]{"TextHorizontalAlignment", TextAlignmentType.Center},
				new Object[]{"TextVerticalAlignment", TextAlignmentType.Center},
				new Object[]{"TextDirection", TextDirectionType.Context},
				new Object[]{ "RotationAngle", 0}
			});
            Console.WriteLine("title.option");
            //================Legend=======================//
            Legend legend = chart.Legend;         
            AssertHelper.AreEqual(FormattingType.Automatic, legend.Area.Formatting, "legend.Area.Formatting");
            ReflectInvoker.invoke("legend", legend, new Object[][]{
			    new Object[]{"Shadow", false},
                new Object[] {"AutoScaleFont", true},
                new Object[] { "BackgroundMode", BackgroundMode.Automatic}
		    });
            Console.WriteLine("Legend");
            ReflectInvoker.invoke("legend.TextFont", legend.TextFont, new Object[][]{
			    new Object[]{"Name", FontNameConstants.zh_SongTi},
			    new Object[]{"Size", 12},
			    new Object[]{"Underline", FontUnderlineType.None},
			    new Object[]{"IsBold", false},
			    new Object[]{"IsItalic", false},
			    new Object[]{"IsStrikeout", false},
			    new Object[]{"IsSubscript", false},
                new Object[]{"IsSuperscript", false}
			});
            Console.WriteLine("Legend.font");
            AssertHelper.equals(Color.Black, legend.TextFont.Color, "legend.TextFont.Color");
            //=================ASeries=======================//
            SeriesCollection nseries = chart.NSeries;
            Series aseries = nseries[0];
            AssertHelper.AreEqual(FormattingType.Automatic, aseries.Area.Formatting, "FormattingType.Automatic");
            ReflectInvoker.invoke("aseries", aseries, new Object[][]{
			    new Object[]{"BubbleSizes", "=Sheet1!$C$2:$C$4"},
			    new Object[]{"Values", "=Sheet1!$B$2:$B$4"},
			    new Object[]{"XValues", "=Sheet1!$A$2:$A$4"},
			    new Object[]{"Name", "=Sheet1!$B$1"},		
                new Object[] {"SizeRepresents", BubbleSizeRepresents.SizeIsArea},
                new Object[]{"ShowNegativeBubbles", true},
			    new Object[]{"IsColorVaried", true},
                new Object[]{"BubbleScale", 100}});
            Console.WriteLine("value");
            AssertHelper.AreEqual(ErrorBarDisplayType.None, aseries.XErrorBar.DisplayType, "aseries.XErrorBar.DisplayType");
            AssertHelper.AreEqual(ErrorBarDisplayType.None, aseries.YErrorBar.DisplayType, "aseries.YErrorBar.DisplayType");
            //====================DataLabels=======================//
            DataLabels datalabels = aseries.DataLabels;
            ReflectInvoker.invoke("datalabels", datalabels, new Object[][]{
			    new Object[]{"ShowSeriesName", false},
			    new Object[]{ "ShowValue", false},
			    new Object[]{"IsBubbleSizeShown", false},
			    new Object[]{"Separator",  DataLabelsSeparatorType.Auto}	});
            Console.WriteLine("datalabels");
            //====================CategoryAxis========================//
            Axis categoryaxis = chart.CategoryAxis;
            AssertHelper.AreEqual(false, categoryaxis.MajorGridLines.IsVisible, "categoryaxis.MajorGridLines.IsVisible");
            AssertHelper.AreEqual(false, categoryaxis.MinorGridLines.IsVisible, "categoryaxis.MinorGridLines.IsVisible");
            ReflectInvoker.invoke("categoryaxis", categoryaxis, new Object[][]{
				new Object[] {"MajorTickMark", TickMarkType.Cross},
				new Object[] {"MinorTickMark", TickMarkType.None},
				new Object[] {"TickLabelPosition", TickLabelPositionType.NextToAxis},				
				new Object[] {"DisplayUnit", DisplayUnitType.None},
				new Object[] {"IsLogarithmic", false},
				new Object[] {"IsPlotOrderReversed", false},
                new Object[] {"IsVisible", true}
				});
            Console.WriteLine("categoryaxis");
            ReflectInvoker.invoke("categoryaxis.TickLabels.Font", categoryaxis.TickLabels.Font, new Object[][]{
			    new Object[]{"Name", FontNameConstants.zh_SongTi},
			    new Object[]{"Size", 12},
			    new Object[]{"Underline", FontUnderlineType.None},
			    new Object[]{"IsBold", false},
			    new Object[]{"IsItalic", false},
			    new Object[]{"IsStrikeout", false},
			    new Object[]{"IsSubscript", false},
                new Object[] {"IsSuperscript", false}
			});
            Console.WriteLine("categoryaxis.tickfont");
            AssertHelper.equals(Color.Black, categoryaxis.TickLabels.Font.Color, "categoryaxis.TickLabels.Font.Color");
            Console.WriteLine("categoryaxis.tickfont1");
            ReflectInvoker.invoke("categoryaxis.TickLabels", categoryaxis.TickLabels, new Object[][]{
			    new Object[] {"AutoScaleFont", true},
                new Object[] { "BackgroundMode", BackgroundMode.Automatic},
                new Object[] {"NumberFormatLinked", true},
                new Object[] {"TextDirection", TextDirectionType.Context},
                new Object[] { "RotationAngle", 0}
            });
            Console.WriteLine("categoryaxis.tick");
            //====================ValueAxis========================//
            Axis valueAxis = chart.ValueAxis;
            AssertHelper.AreEqual(true, valueAxis.MajorGridLines.IsVisible, "valueAxis.MajorGridLines.IsVisible");
            AssertHelper.AreEqual(false, valueAxis.MinorGridLines.IsVisible, "valueAxis.MinorGridLines.IsVisible");
            Console.WriteLine("categoryaxis.tick");
            ReflectInvoker.invoke("valueAxis", valueAxis, new Object[][]{
				new Object[] {"MajorTickMark", TickMarkType.Cross},
				new Object[] {"MinorTickMark", TickMarkType.None},
				new Object[] {"TickLabelPosition", TickLabelPositionType.NextToAxis},
				new Object[] {"DisplayUnit", DisplayUnitType.None},
				new Object[] {"IsLogarithmic", false},
				new Object[] {"IsPlotOrderReversed", false},
                new Object[] {"IsVisible", true}
            });
            ReflectInvoker.invoke("valueAxis.TickLabels.Font", valueAxis.TickLabels.Font, new Object[][]{
			    new Object[]{"Name", FontNameConstants.zh_SongTi},
			    new Object[]{"Size", 12},
			    new Object[]{"Underline", FontUnderlineType.None},
			    new Object[]{"IsBold", false},
			    new Object[]{"IsItalic", false},
			    new Object[]{"IsStrikeout", false},
			    new Object[]{"IsSubscript", false},
                new Object[]{"IsSuperscript", false}
			});
            AssertHelper.equals(Color.Black, valueAxis.TickLabels.Font.Color, "valueAxis.TickLabels.Font.Color");

            ReflectInvoker.invoke(" valueAxis.TickLabels", valueAxis.TickLabels, new Object[][]{
				new Object[] {"AutoScaleFont", true},
                new Object[] { "BackgroundMode", BackgroundMode.Automatic},
                new Object[] {"NumberFormatLinked", true},
                new Object[] {"TextDirection", TextDirectionType.Context},
                new Object[] { "RotationAngle", 0}
            });
        }
```

### See Also

* class [ErrorBar](../../errorbar/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


