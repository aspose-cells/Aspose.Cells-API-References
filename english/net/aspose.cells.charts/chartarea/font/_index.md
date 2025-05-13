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
// Called: ReflectInvoker.invoke("chartArea.TextFont", chartArea.Font, new Object[][]{
        public void ChartArea_Property_Font()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "Charts\\Doughnut.xls");
            Worksheet worksheet = workbook.Worksheets[0];
            Chart chart = worksheet.Charts[0];
            ReflectInvoker.invoke("chart", chart, new Object[][]{
			    new Object[]{"Type", ChartType.Doughnut},
                new Object[] {"IsRectangularCornered", true},
                new Object[] { "ShowLegend", true},
                new Object[] {"FirstSliceAngle", 0}
            });
            ReflectInvoker.invoke("chart.ChartObject", chart.ChartObject, new Object[][]{
                new Object[] { "IsPrintable", true},
			    new Object[]{"IsLocked", true},
                new Object[] {"Placement", PlacementType.Move}});   
            //==============ChartArea==================//
            ChartArea chartArea = chart.ChartArea;
            //AssertHelper.AreEqual(true, chartArea.Border.IsAuto, "chartArea.Border.IsAuto");
            AssertHelper.AreEqual(FormattingType.Automatic, chartArea.Area.Formatting, "chartArea.Area.Formatting");
            ReflectInvoker.invoke("chartArea", chartArea, new Object[][]{
				new Object[]{"Shadow", false},
				new Object[]{"AutoScaleFont", false},
				new Object[] { "BackgroundMode", BackgroundMode.Automatic},
			}); 
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
            //===================Title==============//
            Title title = chart.Title;
            AssertHelper.AreEqual(false, title.Border.IsVisible, "title.Border.IsVisible");
            AssertHelper.AreEqual(FormattingType.None, title.Area.Formatting, "title.Area.Formatting");

            ReflectInvoker.invoke("title", title, new Object[][]{
                  new Object[] {"Text", "Fruit Sales by Region For Years"},
                  new Object[] {"Shadow", false},
			      new Object[] {"AutoScaleFont", false},
			      new Object[] { "BackgroundMode", BackgroundMode.Automatic},
                  new Object[] {"TextHorizontalAlignment", TextAlignmentType.Center},
                  new Object[] {"TextVerticalAlignment", TextAlignmentType.Center},
                  new Object[] {"TextDirection", TextDirectionType.Context},
                  new Object[] { "RotationAngle", 0}
			});  
            ReflectInvoker.invoke("title.TextFont", title.TextFont, new Object[][]{
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
            //================Legend=================//
            Legend legend = chart.Legend;
            //AssertHelper.AreEqual(true, legend.Border.IsAuto, "legend.Border.IsAuto");
            AssertHelper.AreEqual(FormattingType.Automatic, legend.Area.Formatting, "legend.Area.Formatting");
            ReflectInvoker.invoke("legend", legend, new Object[][]{
                new Object[] {"Shadow", false},
                new Object[] {"AutoScaleFont", false},
                new Object[] { "BackgroundMode", BackgroundMode.Automatic},
                new Object[] {"Position", LegendPositionType.Top}
              });
            ReflectInvoker.invoke("legend.TextFont", legend.TextFont, new Object[][]{
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
            //===========PlotArea==================//
            AssertHelper.AreEqual(false, chart.PlotArea.Border.IsVisible, "chart.PlotArea.Border.IsVisible");
            AssertHelper.AreEqual(FormattingType.Automatic, chart.PlotArea.Area.Formatting, "chart.PlotArea.Area.Formatting");
            //============ASeries================//
            SeriesCollection nseries = chart.NSeries;
            Series aseries = nseries[0];
            //AssertHelper.AreEqual(true, aseries.Line.IsAuto, "aseries.Line.IsAuto");
            AssertHelper.AreEqual(FormattingType.Automatic, aseries.Area.Formatting, "aseries.Area.Formatting");
            ReflectInvoker.invoke("aseries", aseries, new Object[][]{
                new Object[] {"PlotOnSecondAxis", false},
                new Object[] {"FirstSliceAngle", (short)0},
                new Object[] {"DoughnutHoleSize", 50},
                new Object[] {"IsColorVaried", true}
               });
          //===============DataLabels===========//
            DataLabels datalabels = aseries.DataLabels;
            ReflectInvoker.invoke("datalabels", datalabels, new Object[][]{
                new Object[] { "ShowSeriesName", false},
                new Object[] { "ShowCategoryName", false},
                new Object[] { "ShowValue", true},
                new Object[] { "ShowPercentage", false},
                new Object[] {"Separator", DataLabelsSeparatorType.Auto},
                new Object[] { "ShowLegendKey", false},
                new Object[] {"Shadow", false},
                //new Object[] {"AutoScaleFont", false},
                new Object[] {"AutoScaleFont", true},
                new Object[] { "BackgroundMode", BackgroundMode.Automatic},
                new Object[] {"NumberFormatLinked", true},
                new Object[] {"TextHorizontalAlignment", TextAlignmentType.Center},
                new Object[] {"TextVerticalAlignment", TextAlignmentType.Center},
                new Object[] {"TextDirection", TextDirectionType.Context},
                new Object[] { "RotationAngle", 0}
             });    
            AssertHelper.AreEqual(false, datalabels.Border.IsVisible, "datalabels.Border.IsVisible");
            AssertHelper.AreEqual(FormattingType.None, datalabels.Area.Formatting, "datalabels.Area.Formatting");
            ReflectInvoker.invoke("datalabels.TextFont", datalabels.TextFont, new Object[][]{
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
        }
```

### See Also

* class [Font](../../../aspose.cells/font/)
* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


