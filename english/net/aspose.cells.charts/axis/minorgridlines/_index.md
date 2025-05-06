---
title: Axis.MinorGridLines
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Represents minor gridlines on a chart axis
type: docs
url: /net/aspose.cells.charts/axis/minorgridlines/
---
## Axis.MinorGridLines property

Represents minor gridlines on a chart axis.

```csharp
public Line MinorGridLines { get; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(false, valueAxis.MinorGridLines.IsVisible, &amp;quot;valueAxis.MinorGridLines.IsVisible&amp;quot;);
[Test]
        public void Property_MinorGridLines()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Charts\\ClusteredBar.xls&quot;);
            Worksheet worksheet = workbook.Worksheets[0];
            Chart chart = worksheet.Charts[0];

            ReflectInvoker.invoke(&quot;chart&quot;, chart, new Object[][]{
			new Object[]{&quot;Type&quot;, ChartType.Bar},
            new Object[] {&quot;IsRectangularCornered&quot;, true},
            new Object[] { &quot;ShowLegend&quot;, true},
            new Object[] { &quot;ShowDataTable&quot;, true}});               
           
            ReflectInvoker.invoke(&quot;chart.ChartObject&quot;, chart.ChartObject, new Object[][]{
                new Object[] { &quot;IsPrintable&quot;, true},
			    new Object[]{&quot;IsLocked&quot;, true},
                new Object[] {&quot;Placement&quot;, PlacementType.MoveAndSize}});               
            //================ChartArea=====================//
            ChartArea chartArea = chart.ChartArea;
            ReflectInvoker.invoke(&quot;chartArea&quot;, chartArea, new Object[][]{
			    new Object[]{&quot;Shadow&quot;, false},
			    new Object[]{&quot;AutoScaleFont&quot;, true},
                new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic}});
          
           // AssertHelper.assertEquals(&quot;chartArea.getBorder.isAuto&quot;, true, chartArea.getBorder().isAuto());          
           AssertHelper.AreEqual(FormattingType.Automatic, chartArea.Area.Formatting, &quot;chartArea.Area.Formatting&quot;);
            
           ReflectInvoker.invoke(&quot;chartArea.TextFont&quot;, chartArea.TextFont, new Object[][]{
               new Object[]{&quot;Name&quot;, FontNameConstants.zh_SongTi},
               new Object[]{&quot;Size&quot;, 12},
               new Object[]{&quot;Underline&quot;, FontUnderlineType.None},
               new Object[]{&quot;IsBold&quot;, false},
               new Object[]{&quot;IsItalic&quot;, false},
               new Object[]{&quot;IsStrikeout&quot;, false},
               new Object[]{&quot;IsSubscript&quot;, false},
               new Object[] {&quot;IsSuperscript&quot;, false}
           });
           AssertHelper.equals(Color.Black, chartArea.TextFont.Color, &quot;chartArea.TextFont.Color&quot;);
            //=================ChartTitle===================//
            //Title title = chart.Title;
            //AssertHelper.AreEqual(false, title.Border.IsVisible, &quot;title.Border.IsVisible&quot;);
            //AssertHelper.AreEqual(FormattingType.None, title.Area.Formatting, &quot;title.Area.Formatting&quot;);
            //ReflectInvoker.invoke(&quot;title&quot;, title, new Object[][]{
            //    new Object[] {&quot;Text&quot;, &quot;Marketing Costs&quot;},
            //    new Object[] {&quot;Shadow&quot;, false},
            //    new Object[] {&quot;AutoScaleFont&quot;, true},
            //    new Object[] {&quot;BackgroundMode&quot;, BackgroundMode.Automatic},
            //    new Object[] {&quot;TextHorizontalAlignment&quot;, TextAlignmentType.Center},
            //    new Object[] {&quot;TextVerticalAlignment&quot;, TextAlignmentType.Center},
            //    new Object[] {&quot;TextDirection&quot;, TextDirectionType.Context},
            //    new Object[] {&quot;RotationAngle&quot;, 0}
            //   });          
            //ReflectInvoker.invoke(&quot;title.TextFont&quot;, title.TextFont, new Object[][]{
            //    new Object[]{&quot;Name&quot;, &quot;Verdana&quot;},
            //    new Object[]{&quot;Size&quot;, 12},
            //    new Object[]{&quot;Underline&quot;, FontUnderlineType.None},            
            //    new Object[]{&quot;IsBold&quot;, false},
            //    new Object[]{&quot;IsItalic&quot;, false},
            //    new Object[]{&quot;IsStrikeout&quot;, false},
            //    new Object[]{&quot;IsSubscript&quot;, false},
            //    new Object[] {&quot;IsSuperscript&quot;, false}
            //});
            //AssertHelper.equals(Color.Black, title.TextFont.Color, &quot;title.TextFont.Color&quot;);
            //================Legend=======================//
            Legend legend = chart.Legend;
          //AssertHelper.assertEquals(&quot;legend.getBorder&quot;, FormattingType.Automatic, legend.Area.Formatting);
          AssertHelper.AreEqual(FormattingType.Automatic, legend.Area.Formatting, &quot;legend.getArea&quot;);

          ReflectInvoker.invoke(&quot;legend&quot;, legend, new Object[][]{
              new Object[] {&quot;Shadow&quot;, false},
              new Object[] {&quot;AutoScaleFont&quot;, true},
              new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic},
              new Object[] {&quot;Position&quot;, LegendPositionType.Right}
           });    
          ReflectInvoker.invoke(&quot;legend.TextFont&quot;, legend.TextFont, new Object[][]{
              new Object[]{&quot;Name&quot;, FontNameConstants.zh_SongTi},
              new Object[]{&quot;Size&quot;, 12},
              new Object[]{&quot;Underline&quot;, FontUnderlineType.None},             
              new Object[]{&quot;IsBold&quot;, false},
              new Object[]{&quot;IsItalic&quot;, false},
              new Object[] {&quot;IsStrikeout&quot;, false},
              new Object[]{&quot;IsSubscript&quot;, false},
              new Object[]{&quot;IsSuperscript&quot;, false}
          });
          AssertHelper.equals(Color.Black, legend.TextFont.Color, &quot;legend.TextFont.Color&quot;);
          //================PlotArea======================//      
          ReflectInvoker.invoke(&quot;chart.PlotArea.Border&quot;, chart.PlotArea.Border, new Object[][]{              
              new Object[] {&quot;Style&quot;, LineType.Solid},
              new Object[] {&quot;Weight&quot;, WeightType.SingleLine}});
          AssertHelper.equals(Color.FromArgb(128, 128, 128), chart.PlotArea.Border.Color, &quot;chart.PlotArea.Border.Color&quot;);
          AssertHelper.equals(Color.FromArgb(192, 192, 192), chart.PlotArea.Area.ForegroundColor, &quot;chart.PlotArea.Area.ForegroundColor&quot;);
          AssertHelper.equals(Color.Black, chart.PlotArea.Area.BackgroundColor, &quot;chart.PlotArea.Area.BackgroundColor&quot;);
          //==============NSeries===========================//
          SeriesCollection nseries = chart.NSeries;
            
          ReflectInvoker.invoke(&quot;nseries&quot;, nseries, new Object[][]{
          new Object[] {&quot;CategoryData&quot;, &quot;=Sheet1!$A$2:$A$4&quot;}});
          //============ASeries============================//
          Series aseries = nseries[0];
          //AssertHelper.assertEquals(&quot;aseries.getBorder&quot;, true, aseries.getBorder().isAuto());
          AssertHelper.AreEqual(FormattingType.Automatic, aseries.Area.Formatting, &quot;aseries.Area.Formatting&quot;);

          ReflectInvoker.invoke(&quot;aseries&quot;, aseries, new Object[][]{
          new Object[] {&quot;Name&quot;, &quot;=Sheet1!$B$1&quot;},
          new Object[] {&quot;Values&quot;, &quot;=Sheet1!$B$2:$B$4&quot;},
          new Object[] {&quot;Overlap&quot;, (short)0},
          new Object[] {&quot;GapWidth&quot;, (short)150},
          new Object[] {&quot;IsColorVaried&quot;, false},
          new Object[] {&quot;Shadow&quot;, false}});    
          //===============DataLabels============//
          DataLabels datalabels = aseries.DataLabels;
          ReflectInvoker.invoke(&quot;datalabels&quot;, datalabels, new Object[][]{
              new Object[] {&quot;ShowSeriesName&quot;, false},
              new Object[] { &quot;ShowCategoryName&quot;, false},
              new Object[] { &quot;ShowValue&quot;, false},
              new Object[] {&quot;Separator&quot;, DataLabelsSeparatorType.Auto}
            });

          ErrorBar errorbar = aseries.YErrorBar;           
          ReflectInvoker.invoke(&quot;errorbar&quot;, errorbar, new Object[][]{
          new Object[] {&quot;DisplayType&quot;, ErrorBarDisplayType.None}});        
          //=========================CategoryAxis=====================//
          Axis categoryAxis = chart.CategoryAxis;
          AssertHelper.AreEqual(false, categoryAxis.MajorGridLines.IsVisible, &quot;categoryAxis.MajorGridLines.IsVisible&quot;);
          AssertHelper.AreEqual(false, categoryAxis.MinorGridLines.IsVisible, &quot;categoryAxis.MinorGridLines.IsVisible&quot;);

          //AssertHelper.assertEquals(&quot;categoryAxis.getAxisLine.isAuto&quot;, true, categoryAxis.getAxisLine().isAuto());
          ReflectInvoker.invoke(&quot;categoryAxis&quot;, categoryAxis, new Object[][]{
              new Object[] {&quot;MajorTickMark&quot;, TickMarkType.Cross},
              new Object[] {&quot;MinorTickMark&quot;, TickMarkType.None},
              new Object[] {&quot;TickLabelPosition&quot;, TickLabelPositionType.NextToAxis},
              new Object[] {&quot;TickLabelSpacing&quot;, 1},
              new Object[] {&quot;TickMarkSpacing&quot;, 1},
              new Object[] {&quot;IsLogarithmic&quot;, false},
              new Object[] {&quot;IsPlotOrderReversed&quot;, false},
              //new Object[] {&quot;isCrossAtMax&quot;, false},
              new Object[] {&quot;IsVisible&quot;, true}
         });           
          AssertHelper.AreEqual(CategoryType.AutomaticScale, categoryAxis.CategoryType, &quot;categoryAxis.CategoryType&quot;);
          ReflectInvoker.invoke(&quot;categoryAxis.TickLabels&quot;, categoryAxis.TickLabels, new Object[][]{
              new Object[]{&quot;AutoScaleFont&quot;, true},
              new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic},
              new Object[] {&quot;NumberFormatLinked&quot;, true},
              new Object[] {&quot;TextDirection&quot;, TextDirectionType.Context},
              new Object[] { &quot;RotationAngle&quot;, 0},
              new Object[] {&quot;Offset&quot;, 100}
          });
          ReflectInvoker.invoke(&quot;categoryAxis.TickLabels.Font&quot;, categoryAxis.TickLabels.Font, new Object[][]{
              new Object[]{&quot;Name&quot;, FontNameConstants.zh_SongTi},
              new Object[]{&quot;Size&quot;, 12},
              new Object[]{&quot;Underline&quot;, FontUnderlineType.None},
              new Object[]{&quot;IsBold&quot;, false},
              new Object[]{&quot;IsItalic&quot;, false},
              new Object[]{&quot;IsStrikeout&quot;, false},
              new Object[] {&quot;IsSubscript&quot;, false},
              new Object[]{&quot;IsSuperscript&quot;, false}
          });
          AssertHelper.equals(Color.Black, categoryAxis.TickLabels.Font.Color, &quot;categoryAxis.TickLabels.Font.Color&quot;);
          //==========================ValueAxis==========================//
          Axis valueAxis = chart.ValueAxis;
          AssertHelper.AreEqual(true, valueAxis.MajorGridLines.IsVisible, &quot;valueAxis.MajorGridLines.IsVisible&quot;);
          AssertHelper.AreEqual(false, valueAxis.MinorGridLines.IsVisible, &quot;valueAxis.MinorGridLines.IsVisible&quot;);

          //AssertHelper.assertEquals(&quot;valueAxis.getAxisLine.isAuto&quot;, true, valueAxis.getAxisLine().isAuto());
          ReflectInvoker.invoke(&quot;valueAxis&quot;, valueAxis, new Object[][]{
              new Object[] {&quot;MajorTickMark&quot;,TickMarkType.Cross},
              new Object[] {&quot;MinorTickMark&quot;, TickMarkType.None},
              new Object[] {&quot;TickLabelPosition&quot;, TickLabelPositionType.NextToAxis},
              new Object[] {&quot;MinValue&quot;, 0d},
              new Object[] {&quot;MaxValue&quot;, 80000d},
              new Object[] {&quot;MajorUnit&quot;, 20000d},
              new Object[] {&quot;MinorUnit&quot;, 4000d},
              new Object[] {&quot;DisplayUnit&quot;, DisplayUnitType.None},
              new Object[] {&quot;IsLogarithmic&quot;, false},
              new Object[] {&quot;IsPlotOrderReversed&quot;, false},
              //new Object[] {&quot;isCrossAtMax&quot;, false},		
              new Object[] {&quot;IsVisible&quot;, true}
         });
           
          ReflectInvoker.invoke(&quot;valueAxis.TickLabels&quot;, valueAxis.TickLabels, new Object[][]{
              new Object[] {&quot;AutoScaleFont&quot;, true},
              new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic},
              new Object[] {&quot;NumberFormatLinked&quot;, true},
              new Object[] { &quot;RotationAngle&quot;, 0},
              new Object[] {&quot;TextDirection&quot;, TextDirectionType.Context}});

          ReflectInvoker.invoke(&quot;valueAxis.TickLabels.Font&quot;, valueAxis.TickLabels.Font, new Object[][]{
              new Object[]{&quot;Name&quot;, FontNameConstants.zh_SongTi},
              new Object[]{&quot;Size&quot;, 12},
              new Object[]{&quot;Underline&quot;, FontUnderlineType.None},
              new Object[]{&quot;IsBold&quot;, false},
              new Object[]{&quot;IsItalic&quot;, false},
              new Object[]{&quot;IsStrikeout&quot;, false},
              new Object[]{&quot;IsSubscript&quot;, false},
              new Object[] {&quot;IsSuperscript&quot;, false}
          });
          AssertHelper.equals(Color.Black, valueAxis.TickLabels.Font.Color, &quot;valueAxis.TickLabels.Font.Color&quot;);
          //AssertHelper.assertEquals(&quot;valueAxis.getMajorGridLines.isAuto&quot;, true, valueAxis.getMajorGridLines().isAuto());

          //================ChartDataTable==================//
          ChartDataTable chartdatatable = chart.ChartDataTable;
          ReflectInvoker.invoke(&quot;ChartDataTable.Border&quot;, chartdatatable.Border, new Object[][]{
                new Object[]{&quot;Color&quot;, Color.Red},
                new Object[] {&quot;Style&quot;, LineType.Dash},
                new Object[] {&quot;Weight&quot;, WeightType.MediumLine}
           });
          ReflectInvoker.invoke(&quot;ChartDataTable&quot;, chartdatatable, new Object[][]{
                new Object[]{&quot;ShowLegendKey&quot;, true},
                new Object[] {&quot;HasBorderHorizontal&quot;, true},
                new Object[] {&quot;HasBorderVertical&quot;, true},
                new Object[] {&quot;HasBorderOutline&quot;, true},
                new Object[] {&quot;AutoScaleFont&quot;, true},
                new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Opaque}
            });
            ReflectInvoker.invoke(&quot;chartdatatable.Font&quot;, chartdatatable.Font, new Object[][]{
              new Object[]{&quot;Name&quot;, FontNameConstants.zh_SongTi},
              new Object[]{&quot;Size&quot;, 12},
              new Object[]{&quot;Underline&quot;, FontUnderlineType.Single},
              new Object[]{&quot;IsBold&quot;, true},
              new Object[]{&quot;IsItalic&quot;, false},
              new Object[]{&quot;IsStrikeout&quot;, false},
              new Object[]{&quot;IsSubscript&quot;, false},
              new Object[] {&quot;IsSuperscript&quot;, true}
          });
            AssertHelper.equals(Color.Blue, chartdatatable.Font.Color, &quot;chartdatatable.Font.Color&quot;);

        }
```

### See Also

* class [Line](../../../aspose.cells.drawing/line/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


