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
[Test]
        public void Property_XErrorBar()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "Charts\\Scatter.xls");
            Worksheet worksheet = workbook.Worksheets[0];
            Chart chart = worksheet.Charts[0];
            ReflectInvoker.invoke("chart", chart, new Object[][]{
			    new Object[]{"Type", ChartType.Scatter},
                new Object[] {"IsRectangularCornered", true},
                new Object[] { "ShowLegend", true},
               });
            ReflectInvoker.invoke("chart.ChartObject", chart.ChartObject, new Object[][]{
                new Object[] { "IsPrintable", true},
			    new Object[]{"IsLocked", true},
                new Object[] {"Placement", PlacementType.Move}});
            //===============ChartArea==================//
            ChartArea chartArea = chart.ChartArea;
            //AssertHelper.assertEquals("chartArea.getBorder.isAuto", true, chartArea.getBorder().isAuto());
            AssertHelper.AreEqual(FormattingType.Automatic, chartArea.Area.Formatting, "chartArea.Area.Formatting");
            ReflectInvoker.invoke("chartArea", chartArea, new Object[][]{
			    new Object[]{"Shadow", false},			
			    new Object[] {"AutoScaleFont", false},
                new Object[] { "BackgroundMode", BackgroundMode.Automatic}});         
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
            //=================Title===================//
            Title title = chart.Title;
            ReflectInvoker.invoke("title.Border", title.Border, new Object[][]{
			    new Object[]{"Style", LineType.Solid},
			    new Object[]{"Color", Color.Red},
			    new Object[]{"Weight",WeightType.HairLine}});
            AssertHelper.AreEqual(FormattingType.None, title.Area.Formatting, "title.Area.Formatting");
            ReflectInvoker.invoke("title", title, new Object[][]{
			    new Object[] {"Text", "Particulate Levels in Rainfall"},
                new Object[] {"Shadow", false},
                new Object[] {"AutoScaleFont", false},
                new Object[] { "BackgroundMode", BackgroundMode.Automatic},
			    new Object[] {"TextHorizontalAlignment", TextAlignmentType.Right},
			    new Object[] {"TextVerticalAlignment", TextAlignmentType.Bottom},
			    new Object[] {"TextDirection", TextDirectionType.LeftToRight},
			    new Object[] { "RotationAngle", -20}});
            ReflectInvoker.invoke("title.TextFont", title.TextFont, new Object[][]{
		        new Object[]{"Name", "Verdana"},
		        new Object[]{"Size", 14},
		        new Object[]{"Underline", FontUnderlineType.None},
		        new Object[]{"Color", Color.Black},
		        new Object[]{"IsBold", true},
		        new Object[]{"IsItalic", false},
		        new Object[]{"IsStrikeout", false},
		        new Object[]{"IsSubscript", false},
                new Object[] {"IsSuperscript", false}
			});           
            //====================Legend===============================//
            Legend legend = chart.Legend;
            //AssertHelper.assertEquals("legend.getBorder.isAuto", true, legend.getBorder().isAuto());
            AssertHelper.AreEqual(FormattingType.Automatic, legend.Area.Formatting, "legend.Area.Formatting");
            ReflectInvoker.invoke("legend", legend, new Object[][]{
                new Object[] {"Shadow", false},
                new Object[] {"AutoScaleFont", false},
                new Object[] { "BackgroundMode", BackgroundMode.Automatic},
			    new Object[]{"Position", LegendPositionType.Top}});                 
            ReflectInvoker.invoke("legend.TextFont", legend.TextFont, new Object[][]{
			    new Object[]{"Name", "Tahoma"},
			    new Object[]{"Size", 10},
			    new Object[]{"Underline", FontUnderlineType.None},
			    new Object[]{"Color", Color.Black},
			    new Object[]{"IsBold", false},
			    new Object[]{"IsItalic", false},
			    new Object[]{"IsStrikeout", false},
			    new Object[]{"IsSubscript", false},
                new Object[] {"IsSuperscript", false}});
            //======================PlotArea===========================//
            ReflectInvoker.invoke("chart.PlotArea.Border", chart.PlotArea.Border, new Object[][]{
			new Object[]{"Style", LineType.Solid},
			new Object[]{"Color", Color.Empty},
			new Object[]{"Weight",WeightType.HairLine}});
            AssertHelper.AreEqual(FormattingType.Automatic, chart.PlotArea.Area.Formatting, "Automatic, chart.PlotArea.Area.Formatting");
            //=====================NSeries===========================//
            SeriesCollection nseries = chart.NSeries;
            //ReflectInvoker.invoke("nseries", nseries, new Object[][]{
            //    new Object[]{"CategoryData", "=Scatter!$B$2:$B$10"}
            //});
            //====================ASeries===========================//
            Series aseries = nseries[0];
            AssertHelper.AreEqual(false, aseries.Border.IsVisible, "aseries.Line.IsVisible");
            ReflectInvoker.invoke("aseries", aseries, new Object[][]{
				new Object[]{"Name", "Particulate"},
				new Object[]{"XValues", "=Scatter!$A$2:$A$10"},
                new Object[]{"Values", "=Scatter!$B$2:$B$10"},
				new Object[]{"IsColorVaried", false},
                //new Object[]{"MarkerStyle", ChartMarkerType.Diamond},
				//new Object[]{"MarkerForegroundColor", Color.Black},
				//new Object[]{"MarkerBackgroundColor", Color.Black},
				//new Object[]{"MarkerSize", 5},
                new Object[] {"Shadow", false}
			});
            AssertHelper.AreEqual(ChartMarkerType.Diamond, aseries.Marker.MarkerStyle, "aseries.Marker.MarkerStyle");
            AssertHelper.IsTrue(Util.CompareColor(Color.FromArgb(0x80), aseries.Marker.ForegroundColor), "aseries.Marker.ForegroundColor");
            AssertHelper.IsTrue(Util.CompareColor(Color.FromArgb(0x80), aseries.Marker.BackgroundColor), "aseries.Marker.BackgroundColor");
            //AssertHelper.AreEqual(Color.FromArgb(0x80), aseries.Marker.ForegroundColor, "aseries.Marker.ForegroundColor");
            //AssertHelper.AreEqual(Color.FromArgb(0x80), aseries.Marker.BackgroundColor, "aseries.Marker.BackgroundColor");
            AssertHelper.AreEqual(5, aseries.Marker.MarkerSize, "aseries.Marker.MarkerSize");

            AssertHelper.AreEqual(ErrorBarDisplayType.None, aseries.XErrorBar.DisplayType, "aseries.XErrorBar.DisplayType");
            AssertHelper.AreEqual(ErrorBarDisplayType.None, aseries.YErrorBar.DisplayType, "aseries.YErrorBar.DisplayType");
            //====================DataLabels=======================//
            DataLabels datalabels = aseries.DataLabels;
            ReflectInvoker.invoke("datalabels", datalabels, new Object[][]{
			new Object[]{ "ShowSeriesName", false},
			new Object[]{ "ShowValue", false},
			new Object[]{"Separator", DataLabelsSeparatorType.Auto}});
            //================CategoryAxis========================//
            Axis categoryAxis = chart.CategoryAxis;
           // AssertHelper.assertEquals("valuexAxis.getAxisLine.isAuto", true, valuexAxis.getAxisLine().isAuto());
            ReflectInvoker.invoke("categoryAxis", categoryAxis, new Object[][]{
				new Object[] {"MajorTickMark", TickMarkType.Cross},
				new Object[] {"MinorTickMark", TickMarkType.None},
				new Object[] {"TickLabelPosition", TickLabelPositionType.NextToAxis},
				new Object[] {"DisplayUnit", DisplayUnitType.None},
				new Object[] {"IsLogarithmic", false},
				new Object[] {"IsPlotOrderReversed", false},
				//new Object[] {"isCrossAtMax", false},
                new Object[] {"IsVisible", true}
				});
            AssertHelper.AreEqual(false, categoryAxis.MajorGridLines.IsVisible, "categoryAxis.MajorGridLines.IsVisible");
            AssertHelper.AreEqual(false, categoryAxis.MinorGridLines.IsVisible, "categoryAxis.MinorGridLines.IsVisible");
            ReflectInvoker.invoke("categoryAxis.TickLabels", categoryAxis.TickLabels, new Object[][]{
				new Object[] {"AutoScaleFont", false},
                new Object[] { "BackgroundMode",  BackgroundMode.Automatic},
                new Object[] {"NumberFormatLinked", true},
                new Object[] {"TextDirection", TextDirectionType.Context},
                new Object[] { "RotationAngle", 0}
              });
            ReflectInvoker.invoke("categoryAxis.TickLabels.Font", categoryAxis.TickLabels.Font, new Object[][]{
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
            //==========//
            Title categoryTitle = categoryAxis.Title;
            AssertHelper.AreEqual(false, categoryTitle.Border.IsVisible, "categoryAxis.Title.Border.IsVisible");
            AssertHelper.AreEqual(FormattingType.None, categoryTitle.Area.Formatting, "categoryAxis.Title.Area.Formatting");
            ReflectInvoker.invoke("categoryAxis.Title", categoryTitle, new Object[][]{
				new Object[] {"Text", "Daily Rainfall"},
                new Object[] {"Shadow", false},
                new Object[] {"AutoScaleFont", false},
                new Object[] { "BackgroundMode", BackgroundMode.Automatic},
				new Object[] {"TextHorizontalAlignment", TextAlignmentType.Center},
				new Object[] {"TextVerticalAlignment", TextAlignmentType.Center},
				new Object[] {"TextDirection", TextDirectionType.Context},
				new Object[] { "RotationAngle", 0}
			});
            ReflectInvoker.invoke("categoryAxis.Title.TextFont", categoryTitle.Font, new Object[][]{
			    new Object[]{"Name", "Arial"},
			    new Object[]{"Size", 10},
			    new Object[]{"Underline", FontUnderlineType.None},
			    new Object[]{"Color", Color.Black},
			    new Object[]{"IsBold", true},
			    new Object[]{"IsItalic", false},
			    new Object[]{"IsStrikeout", false},
			    new Object[]{"IsSubscript", false},
                new Object[] {"IsSuperscript", false}
			});           
            //================ValueAxis========================//
            Axis valueAxis = chart.ValueAxis;
            ReflectInvoker.invoke("valueAxis.AxisLine", valueAxis.AxisLine, new Object[][]{
		        new Object[]{"Style", LineType.Solid},
		        new Object[]{"Color", Color.Empty},
		        new Object[]{"Weight",WeightType.HairLine}});
            ReflectInvoker.invoke("valueAxis", valueAxis, new Object[][]{
				new Object[] {"MajorTickMark", TickMarkType.Cross},
				new Object[] {"MinorTickMark", TickMarkType.None},
				new Object[] {"TickLabelPosition", TickLabelPositionType.NextToAxis},
				new Object[] {"DisplayUnit", DisplayUnitType.None},
				new Object[] {"IsLogarithmic", false},
				new Object[] {"IsPlotOrderReversed", false},
				//new Object[] {"isCrossAtMax", false},
                new Object[] {"IsVisible", true}
				});           
            ReflectInvoker.invoke("valueAxis.TickLabels", valueAxis.TickLabels, new Object[][]{
                new Object[] {"AutoScaleFont", false},
				new Object[] {"NumberFormatLinked", true},
                new Object[] { "BackgroundMode", BackgroundMode.Automatic},
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
                new Object[] {"IsSuperscript", false}
			});
            AssertHelper.AreEqual(false, valueAxis.MajorGridLines.IsVisible, "valueAxis.MajorGridLines.IsVisible");
            AssertHelper.AreEqual(false, valueAxis.MinorGridLines.IsVisible, "valueAxis.MinorGridLines.IsVisible");
            //==========//
            Title valueAxisTitle = valueAxis.Title;
            AssertHelper.AreEqual(false, valueAxisTitle.Border.IsVisible, "valueAxis.Title.Border.IsVisible");
            AssertHelper.AreEqual(FormattingType.None, valueAxisTitle.Area.Formatting, "valueAxisTitle.Area.Formatting");
           
            ReflectInvoker.invoke("valueAxis.TextFont", valueAxisTitle.Font, new Object[][]{
			    new Object[]{"Name", "Arial"},
			    new Object[]{"Size", 10},
			    new Object[]{"Underline", FontUnderlineType.None},
			    new Object[]{"Color", Color.Black},
			    new Object[]{"IsBold", true},
			    new Object[]{"IsItalic", false},
			    new Object[]{"IsStrikeout", false},
			    new Object[]{"IsSubscript", false},
                new Object[] {"IsSuperscript", false}
			});
            ReflectInvoker.invoke("valueAxis", valueAxisTitle, new Object[][]{
				new Object[]{"Text", "Particulate"},
                new Object[] {"Shadow", false},
                new Object[] {"AutoScaleFont", false}, 
                new Object[] { "BackgroundMode", BackgroundMode.Automatic},
				new Object[]{"TextHorizontalAlignment", TextAlignmentType.Center},
				new Object[] {"TextVerticalAlignment", TextAlignmentType.Center},
				new Object[] {"TextDirection", TextDirectionType.Context},
				new Object[] { "RotationAngle", 90}
			});	


        }
```

### See Also

* class [ErrorBar](../../errorbar/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


