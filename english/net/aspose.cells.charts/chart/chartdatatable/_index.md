---
title: Chart.ChartDataTable
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Represents the chart data table
type: docs
url: /net/aspose.cells.charts/chart/chartdatatable/
---
## Chart.ChartDataTable property

Represents the chart data table.

```csharp
public ChartDataTable ChartDataTable { get; }
```

### Examples

```csharp
// Called: ChartDataTable chartdatatable = chart.ChartDataTable;
        public void Chart_Property_ChartDataTable()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "Charts\\ClusteredBar.xls");
            Worksheet worksheet = workbook.Worksheets[0];
            Chart chart = worksheet.Charts[0];

            ReflectInvoker.invoke("chart", chart, new Object[][]{
			new Object[]{"Type", ChartType.Bar},
            new Object[] {"IsRectangularCornered", true},
            new Object[] { "ShowLegend", true},
            new Object[] { "ShowDataTable", true}});               
           
            ReflectInvoker.invoke("chart.ChartObject", chart.ChartObject, new Object[][]{
                new Object[] { "IsPrintable", true},
			    new Object[]{"IsLocked", true},
                new Object[] {"Placement", PlacementType.MoveAndSize}});               
            //================ChartArea=====================//
            ChartArea chartArea = chart.ChartArea;
            ReflectInvoker.invoke("chartArea", chartArea, new Object[][]{
			    new Object[]{"Shadow", false},
			    new Object[]{"AutoScaleFont", true},
                new Object[] { "BackgroundMode", BackgroundMode.Automatic}});
          
           // AssertHelper.assertEquals("chartArea.getBorder.isAuto", true, chartArea.getBorder().isAuto());          
           AssertHelper.AreEqual(FormattingType.Automatic, chartArea.Area.Formatting, "chartArea.Area.Formatting");
            
           ReflectInvoker.invoke("chartArea.TextFont", chartArea.TextFont, new Object[][]{
               new Object[]{"Name", FontNameConstants.zh_SongTi},
               new Object[]{"Size", 12},
               new Object[]{"Underline", FontUnderlineType.None},
               new Object[]{"IsBold", false},
               new Object[]{"IsItalic", false},
               new Object[]{"IsStrikeout", false},
               new Object[]{"IsSubscript", false},
               new Object[] {"IsSuperscript", false}
           });
           AssertHelper.equals(Color.Black, chartArea.TextFont.Color, "chartArea.TextFont.Color");
            //=================ChartTitle===================//
            //Title title = chart.Title;
            //AssertHelper.AreEqual(false, title.Border.IsVisible, "title.Border.IsVisible");
            //AssertHelper.AreEqual(FormattingType.None, title.Area.Formatting, "title.Area.Formatting");
            //ReflectInvoker.invoke("title", title, new Object[][]{
            //    new Object[] {"Text", "Marketing Costs"},
            //    new Object[] {"Shadow", false},
            //    new Object[] {"AutoScaleFont", true},
            //    new Object[] {"BackgroundMode", BackgroundMode.Automatic},
            //    new Object[] {"TextHorizontalAlignment", TextAlignmentType.Center},
            //    new Object[] {"TextVerticalAlignment", TextAlignmentType.Center},
            //    new Object[] {"TextDirection", TextDirectionType.Context},
            //    new Object[] {"RotationAngle", 0}
            //   });          
            //ReflectInvoker.invoke("title.TextFont", title.TextFont, new Object[][]{
            //    new Object[]{"Name", "Verdana"},
            //    new Object[]{"Size", 12},
            //    new Object[]{"Underline", FontUnderlineType.None},            
            //    new Object[]{"IsBold", false},
            //    new Object[]{"IsItalic", false},
            //    new Object[]{"IsStrikeout", false},
            //    new Object[]{"IsSubscript", false},
            //    new Object[] {"IsSuperscript", false}
            //});
            //AssertHelper.equals(Color.Black, title.TextFont.Color, "title.TextFont.Color");
            //================Legend=======================//
            Legend legend = chart.Legend;
          //AssertHelper.assertEquals("legend.getBorder", FormattingType.Automatic, legend.Area.Formatting);
          AssertHelper.AreEqual(FormattingType.Automatic, legend.Area.Formatting, "legend.getArea");

          ReflectInvoker.invoke("legend", legend, new Object[][]{
              new Object[] {"Shadow", false},
              new Object[] {"AutoScaleFont", true},
              new Object[] { "BackgroundMode", BackgroundMode.Automatic},
              new Object[] {"Position", LegendPositionType.Right}
           });    
          ReflectInvoker.invoke("legend.TextFont", legend.TextFont, new Object[][]{
              new Object[]{"Name", FontNameConstants.zh_SongTi},
              new Object[]{"Size", 12},
              new Object[]{"Underline", FontUnderlineType.None},             
              new Object[]{"IsBold", false},
              new Object[]{"IsItalic", false},
              new Object[] {"IsStrikeout", false},
              new Object[]{"IsSubscript", false},
              new Object[]{"IsSuperscript", false}
          });
          AssertHelper.equals(Color.Black, legend.TextFont.Color, "legend.TextFont.Color");
          //================PlotArea======================//      
          ReflectInvoker.invoke("chart.PlotArea.Border", chart.PlotArea.Border, new Object[][]{              
              new Object[] {"Style", LineType.Solid},
              new Object[] {"Weight", WeightType.SingleLine}});
          AssertHelper.equals(Color.FromArgb(128, 128, 128), chart.PlotArea.Border.Color, "chart.PlotArea.Border.Color");
          AssertHelper.equals(Color.FromArgb(192, 192, 192), chart.PlotArea.Area.ForegroundColor, "chart.PlotArea.Area.ForegroundColor");
          AssertHelper.equals(Color.Black, chart.PlotArea.Area.BackgroundColor, "chart.PlotArea.Area.BackgroundColor");
          //==============NSeries===========================//
          SeriesCollection nseries = chart.NSeries;
            
          ReflectInvoker.invoke("nseries", nseries, new Object[][]{
          new Object[] {"CategoryData", "=Sheet1!$A$2:$A$4"}});
          //============ASeries============================//
          Series aseries = nseries[0];
          //AssertHelper.assertEquals("aseries.getBorder", true, aseries.getBorder().isAuto());
          AssertHelper.AreEqual(FormattingType.Automatic, aseries.Area.Formatting, "aseries.Area.Formatting");

          ReflectInvoker.invoke("aseries", aseries, new Object[][]{
          new Object[] {"Name", "=Sheet1!$B$1"},
          new Object[] {"Values", "=Sheet1!$B$2:$B$4"},
          new Object[] {"Overlap", (short)0},
          new Object[] {"GapWidth", (short)150},
          new Object[] {"IsColorVaried", false},
          new Object[] {"Shadow", false}});    
          //===============DataLabels============//
          DataLabels datalabels = aseries.DataLabels;
          ReflectInvoker.invoke("datalabels", datalabels, new Object[][]{
              new Object[] {"ShowSeriesName", false},
              new Object[] { "ShowCategoryName", false},
              new Object[] { "ShowValue", false},
              new Object[] {"Separator", DataLabelsSeparatorType.Auto}
            });

          ErrorBar errorbar = aseries.YErrorBar;           
          ReflectInvoker.invoke("errorbar", errorbar, new Object[][]{
          new Object[] {"DisplayType", ErrorBarDisplayType.None}});        
          //=========================CategoryAxis=====================//
          Axis categoryAxis = chart.CategoryAxis;
          AssertHelper.AreEqual(false, categoryAxis.MajorGridLines.IsVisible, "categoryAxis.MajorGridLines.IsVisible");
          AssertHelper.AreEqual(false, categoryAxis.MinorGridLines.IsVisible, "categoryAxis.MinorGridLines.IsVisible");

          //AssertHelper.assertEquals("categoryAxis.getAxisLine.isAuto", true, categoryAxis.getAxisLine().isAuto());
          ReflectInvoker.invoke("categoryAxis", categoryAxis, new Object[][]{
              new Object[] {"MajorTickMark", TickMarkType.Cross},
              new Object[] {"MinorTickMark", TickMarkType.None},
              new Object[] {"TickLabelPosition", TickLabelPositionType.NextToAxis},
              new Object[] {"TickLabelSpacing", 1},
              new Object[] {"TickMarkSpacing", 1},
              new Object[] {"IsLogarithmic", false},
              new Object[] {"IsPlotOrderReversed", false},
              //new Object[] {"isCrossAtMax", false},
              new Object[] {"IsVisible", true}
         });           
          AssertHelper.AreEqual(CategoryType.AutomaticScale, categoryAxis.CategoryType, "categoryAxis.CategoryType");
          ReflectInvoker.invoke("categoryAxis.TickLabels", categoryAxis.TickLabels, new Object[][]{
              new Object[]{"AutoScaleFont", true},
              new Object[] { "BackgroundMode", BackgroundMode.Automatic},
              new Object[] {"NumberFormatLinked", true},
              new Object[] {"TextDirection", TextDirectionType.Context},
              new Object[] { "RotationAngle", 0},
              new Object[] {"Offset", 100}
          });
          ReflectInvoker.invoke("categoryAxis.TickLabels.Font", categoryAxis.TickLabels.Font, new Object[][]{
              new Object[]{"Name", FontNameConstants.zh_SongTi},
              new Object[]{"Size", 12},
              new Object[]{"Underline", FontUnderlineType.None},
              new Object[]{"IsBold", false},
              new Object[]{"IsItalic", false},
              new Object[]{"IsStrikeout", false},
              new Object[] {"IsSubscript", false},
              new Object[]{"IsSuperscript", false}
          });
          AssertHelper.equals(Color.Black, categoryAxis.TickLabels.Font.Color, "categoryAxis.TickLabels.Font.Color");
          //==========================ValueAxis==========================//
          Axis valueAxis = chart.ValueAxis;
          AssertHelper.AreEqual(true, valueAxis.MajorGridLines.IsVisible, "valueAxis.MajorGridLines.IsVisible");
          AssertHelper.AreEqual(false, valueAxis.MinorGridLines.IsVisible, "valueAxis.MinorGridLines.IsVisible");

          //AssertHelper.assertEquals("valueAxis.getAxisLine.isAuto", true, valueAxis.getAxisLine().isAuto());
          ReflectInvoker.invoke("valueAxis", valueAxis, new Object[][]{
              new Object[] {"MajorTickMark",TickMarkType.Cross},
              new Object[] {"MinorTickMark", TickMarkType.None},
              new Object[] {"TickLabelPosition", TickLabelPositionType.NextToAxis},
              new Object[] {"MinValue", 0d},
              new Object[] {"MaxValue", 80000d},
              new Object[] {"MajorUnit", 20000d},
              new Object[] {"MinorUnit", 4000d},
              new Object[] {"DisplayUnit", DisplayUnitType.None},
              new Object[] {"IsLogarithmic", false},
              new Object[] {"IsPlotOrderReversed", false},
              //new Object[] {"isCrossAtMax", false},		
              new Object[] {"IsVisible", true}
         });
           
          ReflectInvoker.invoke("valueAxis.TickLabels", valueAxis.TickLabels, new Object[][]{
              new Object[] {"AutoScaleFont", true},
              new Object[] { "BackgroundMode", BackgroundMode.Automatic},
              new Object[] {"NumberFormatLinked", true},
              new Object[] { "RotationAngle", 0},
              new Object[] {"TextDirection", TextDirectionType.Context}});

          ReflectInvoker.invoke("valueAxis.TickLabels.Font", valueAxis.TickLabels.Font, new Object[][]{
              new Object[]{"Name", FontNameConstants.zh_SongTi},
              new Object[]{"Size", 12},
              new Object[]{"Underline", FontUnderlineType.None},
              new Object[]{"IsBold", false},
              new Object[]{"IsItalic", false},
              new Object[]{"IsStrikeout", false},
              new Object[]{"IsSubscript", false},
              new Object[] {"IsSuperscript", false}
          });
          AssertHelper.equals(Color.Black, valueAxis.TickLabels.Font.Color, "valueAxis.TickLabels.Font.Color");
          //AssertHelper.assertEquals("valueAxis.getMajorGridLines.isAuto", true, valueAxis.getMajorGridLines().isAuto());

          //================ChartDataTable==================//
          ChartDataTable chartdatatable = chart.ChartDataTable;
          ReflectInvoker.invoke("ChartDataTable.Border", chartdatatable.Border, new Object[][]{
                new Object[]{"Color", Color.Red},
                new Object[] {"Style", LineType.Dash},
                new Object[] {"Weight", WeightType.MediumLine}
           });
          ReflectInvoker.invoke("ChartDataTable", chartdatatable, new Object[][]{
                new Object[]{"ShowLegendKey", true},
                new Object[] {"HasBorderHorizontal", true},
                new Object[] {"HasBorderVertical", true},
                new Object[] {"HasBorderOutline", true},
                new Object[] {"AutoScaleFont", true},
                new Object[] { "BackgroundMode", BackgroundMode.Opaque}
            });
            ReflectInvoker.invoke("chartdatatable.Font", chartdatatable.Font, new Object[][]{
              new Object[]{"Name", FontNameConstants.zh_SongTi},
              new Object[]{"Size", 12},
              new Object[]{"Underline", FontUnderlineType.Single},
              new Object[]{"IsBold", true},
              new Object[]{"IsItalic", false},
              new Object[]{"IsStrikeout", false},
              new Object[]{"IsSubscript", false},
              new Object[] {"IsSuperscript", true}
          });
            AssertHelper.equals(Color.Blue, chartdatatable.Font.Color, "chartdatatable.Font.Color");

        }
```

### See Also

* class [ChartDataTable](../../chartdatatable/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


