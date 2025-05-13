---
title: Axis.AxisLine
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Gets the appearance of an Axis
type: docs
url: /net/aspose.cells.charts/axis/axisline/
---
## Axis.AxisLine property

Gets the appearance of an Axis.

```csharp
public Line AxisLine { get; }
```

### Examples

```csharp
// Called: ReflectInvoker.invoke("valueAxis.AxisLine", valueAxis.AxisLine, new Object[][]{
        public void Axis_Property_AxisLine()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "Charts\\FilledRadar.xls");
            Worksheet worksheet = workbook.Worksheets[0];
            Chart chart = worksheet.Charts[0];
            ReflectInvoker.invoke("chart", chart, new Object[][]{
			    new Object[]{"Type", ChartType.RadarFilled},
                new Object[] {"IsRectangularCornered", true},              
                new Object[] {"FirstSliceAngle", 0},
                new Object[] { "ShowLegend", true}});          
            ReflectInvoker.invoke("chart.ChartObject", chart.ChartObject, new Object[][]{
                new Object[] { "IsPrintable", true},
			    new Object[]{"IsLocked", true},
                new Object[] {"Placement", PlacementType.Move}});   
            //============ChartArea===============//
            ChartArea chartArea = chart.ChartArea;
            //AssertHelper.AreEqual(true, chartArea.Border.IsAuto, "chartArea.Border.IsAuto");
            AssertHelper.AreEqual(FormattingType.Automatic, chartArea.Area.Formatting, "chartArea.Area.Formatting");
            ReflectInvoker.invoke("chartArea.TextFont", chartArea.Font, new Object[][]{
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
            ReflectInvoker.invoke("chartArea", chartArea, new Object[][]{
				new Object[]{"Shadow", false},
				new Object[]{"AutoScaleFont", false},
				new Object[] { "BackgroundMode", BackgroundMode.Automatic},
			});    
            //=============Title======================//
            Title title = chart.Title;
            AssertHelper.AreEqual(false, title.Border.IsVisible, "title.Border.IsVisible");
            AssertHelper.AreEqual(FormattingType.None, title.Area.Formatting, "title.Area.Formatting");
            ReflectInvoker.invoke("title", title, new Object[][]{
                  new Object[] {"Text", "Nutritional Analysis"},
                  new Object[] {"Shadow", false},
			      new Object[]{"AutoScaleFont", false},
			      new Object[]{ "BackgroundMode", BackgroundMode.Automatic},
                  new Object[] {"TextHorizontalAlignment", TextAlignmentType.Center},
                  new Object[] {"TextVerticalAlignment", TextAlignmentType.Center},
                  new Object[] {"TextDirection", TextDirectionType.Context},
                  new Object[] { "RotationAngle", 0}
			});         
            ReflectInvoker.invoke("title.TextFont", title.Font, new Object[][]{
			    new Object[]{"Name", "Arial"},
			    new Object[]{"Size", 12},
			    new Object[]{"Underline", FontUnderlineType.None},
			    new Object[]{"Color", Color.Black},
			    new Object[]{"IsBold", true},
			    new Object[]{"IsItalic", false},
			    new Object[]{"IsStrikeout", false},
			    new Object[]{"IsSubscript", false},
                new Object[] {"IsSuperscript", false}
			});
            //=============Legend=====================//
            Legend legend = chart.Legend;
            //AssertHelper.AreEqual(true, legend.Border.IsAuto, "legend.Border.IsAuto");
            AssertHelper.AreEqual(FormattingType.Automatic, legend.Area.Formatting, "legend.Area.Formatting");
            ReflectInvoker.invoke("legend", legend, new Object[][]{
                new Object[] {"Shadow", false},
                new Object[] {"AutoScaleFont", false},
                new Object[] { "BackgroundMode", BackgroundMode.Automatic},
                new Object[] {"Position", LegendPositionType.Right}
              });
            ReflectInvoker.invoke("legend.TextFont", legend.Font, new Object[][]{
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
            //==========PlotArea=================//
            AssertHelper.AreEqual(false, chart.PlotArea.Border.IsVisible, "chart.PlotArea.Border.IsVisible");
            AssertHelper.AreEqual(FormattingType.Automatic, chart.PlotArea.Area.Formatting, "chart.PlotArea.Area.Formatting");
            //=================NSeries==========================//
            SeriesCollection nseries = chart.NSeries;
            ReflectInvoker.invoke("nseries", nseries, new Object[][]{
				new Object[]{"CategoryData", "=Sheet1!$B$1:$G$1"},
				new Object[]{"Count", 3}
			});
            //===================ASeries=====================//
            Series aseries = nseries[0];
            ReflectInvoker.invoke("aseries", aseries, new Object[][]{
				new Object[]{"Name", "Brand A"},
				new Object[]{"Values", "=Sheet1!$B$2:$G$2"},
				new Object[]{"PlotOnSecondAxis", false}
			});
            //AssertHelper.assertEquals("aseries.getBorder.isAuto", true, aseries.getBorder().isAuto());
            AssertHelper.AreEqual(FormattingType.Automatic, aseries.Area.Formatting, "aseries.Area.Formatting");
            //===================DataLabels=====================//
            DataLabels datalabels = aseries.DataLabels;
            ReflectInvoker.invoke("datalabels", datalabels, new Object[][]{
				new Object[]{ "ShowSeriesName", false},
				new Object[]{ "ShowCategoryName", false},
				new Object[]{ "ShowValue", false},
				new Object[]{ "SeparatorType", DataLabelsSeparatorType.Auto},		
			});	
            //===========valueAxis=======================//
            Axis valueAxis = chart.ValueAxis;
            ReflectInvoker.invoke("valueAxis.AxisLine", valueAxis.AxisLine, new Object[][]{
			    new Object[] {"Style", LineType.Solid},
                new Object[] {"Color", Color.Empty},
                new Object[] {"Weight", WeightType.HairLine}
              });
            ReflectInvoker.invoke("valueAxis", valueAxis, new Object[][]{
			    new Object[] {"MinorTickMark", TickMarkType.None},
                new Object[] {"TickLabelPosition", TickLabelPositionType.NextToAxis},
                new Object[] {"DisplayUnit", DisplayUnitType.None},
                new Object[] {"IsLogarithmic", false},
                new Object[] {"IsVisible", true}
            });
            AssertHelper.AreEqual(true, valueAxis.MajorGridLines.IsVisible, "valueAxis.MajorGridLines.IsVisible");
            AssertHelper.AreEqual(false, valueAxis.MinorGridLines.IsVisible, "valueAxis.MinorGridLines.IsVisible");
            ReflectInvoker.invoke("valueAxis.TickLabels", valueAxis.TickLabels, new Object[][]{
                new Object[] {"AutoScaleFont", false},
                new Object[] { "BackgroundMode", BackgroundMode.Automatic},
			    new Object[] {"NumberFormatLinked", true},
                new Object[] { "RotationAngle", 0},
                new Object[] {"TextDirection", TextDirectionType.Context}                
            });
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
            //====================CategoryAxis=======================//
            Axis categoryAxis = chart.CategoryAxis;
            TickLabels ticklabels = categoryAxis.TickLabels;
            ReflectInvoker.invoke("categoryAxis.TickLabels.Font", ticklabels.Font, new Object[][]{
			    new Object[]{"Name", "Tahoma"},
			    new Object[]{"Size", 10},
			    new Object[]{"Underline", FontUnderlineType.None},
			    new Object[]{"Color", Color.Black},
			    new Object[]{"IsBold", false},
			    new Object[]{"IsItalic", false},
			    new Object[]{"IsStrikeout", false},
			    new Object[]{"IsSubscript", false},
                new Object[] {"IsSuperscript", false}});
            ReflectInvoker.invoke("categoryAxis.Title", ticklabels, new Object[][]{
                new Object[] {"AutoScaleFont", false},
                new Object[] { "BackgroundMode", BackgroundMode.Automatic},
			    new Object[] { "RotationAngle", 30},
			    new Object[] {"TextDirection", TextDirectionType.Context}});  
        }
```

### See Also

* class [Line](../../../aspose.cells.drawing/line/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


