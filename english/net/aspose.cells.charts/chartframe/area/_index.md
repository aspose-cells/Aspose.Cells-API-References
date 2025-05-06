---
title: ChartFrame.Area
second_title: Aspose.Cells for .NET API Reference
description: ChartFrame property. Gets the area
type: docs
url: /net/aspose.cells.charts/chartframe/area/
---
## ChartFrame.Area property

Gets the `area`.

```csharp
public virtual Area Area { get; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(FormattingType.Automatic, chartarea.Area.Formatting, &amp;quot;chartarea.Area.Formatting&amp;quot;);
[Test]
        public void Property_Area()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Charts\\PieofPie.xls&quot;);
            Worksheet worksheet = workbook.Worksheets[1];
            Chart chart = worksheet.Charts[0];
            ReflectInvoker.invoke(&quot;chart&quot;, chart, new Object[][]{
			    new Object[]{&quot;Type&quot;, ChartType.PiePie},
                new Object[] { &quot;ShowLegend&quot;, true}
               });   
            //================ChartArea=================//
            ChartArea chartarea = chart.ChartArea;            
            //AssertHelper.AreEqual(true, chartarea.Border, 
            AssertHelper.AreEqual(FormattingType.Automatic, chartarea.Area.Formatting, &quot;chartarea.Area.Formatting&quot;);
            ReflectInvoker.invoke(&quot;chartarea&quot;, chartarea, new Object[][]{
			    new Object[] {&quot;Shadow&quot;, false},
                new Object[] {&quot;AutoScaleFont&quot;, false},
                new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic}
            });        
            Aspose.Cells.Font font = chartarea.TextFont;
            ReflectInvoker.invoke(&quot;chartarea.TextFont&quot;, font, new Object[][]{
			    new Object[] {&quot;Name&quot;, &quot;Tahoma&quot;},
                new Object[] {&quot;Size&quot;, 10},
                new Object[] {&quot;Underline&quot;, FontUnderlineType.None},
                new Object[] {&quot;IsBold&quot;, false},
                new Object[] {&quot;IsItalic&quot;, false},
                new Object[] {&quot;IsStrikeout&quot;, false},
                new Object[] {&quot;IsSubscript&quot;, false},
                new Object[] {&quot;IsSuperscript&quot;, false}
             });
            AssertHelper.equals(Color.Black, font.Color, &quot;chartarea.TextFont.Color&quot;);
            //================ChartTitle=================//
            Title title = chart.Title;
            AssertHelper.AreEqual(false, title.Border.IsVisible, &quot;chart.title.Border&quot;);
            AssertHelper.AreEqual(FormattingType.None, title.Area.Formatting, &quot;chart.title.Area&quot;);
            ReflectInvoker.invoke(&quot;title&quot;, title, new Object[][]{
                new Object[] {&quot;Text&quot;, &quot;Sales By Region&quot;},
			    new Object[] {&quot;Shadow&quot;, false},
                new Object[] {&quot;AutoScaleFont&quot;, false},
                new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic},
                new Object[] {&quot;TextHorizontalAlignment&quot;, TextAlignmentType.Center},
                new Object[] {&quot;TextVerticalAlignment&quot;, TextAlignmentType.Center},
                new Object[] {&quot;TextDirection&quot;, TextDirectionType.Context},
                new Object[] { &quot;RotationAngle&quot;, 0}
            });
            font = title.TextFont;
            ReflectInvoker.invoke(&quot;title.TextFont&quot;, font, new Object[][]{
			    new Object[] {&quot;Name&quot;, &quot;Arial&quot;},
                new Object[] {&quot;Size&quot;, 12},
                new Object[] {&quot;Underline&quot;, FontUnderlineType.None},
                new Object[] {&quot;IsBold&quot;, true},
                new Object[] {&quot;IsItalic&quot;, false},
                new Object[] {&quot;IsStrikeout&quot;, false},
                new Object[] {&quot;IsSubscript&quot;, false},
                new Object[] {&quot;IsSuperscript&quot;, false}
             });           
            AssertHelper.equals(Color.Black, font.Color, &quot;title.TextFont.Color&quot;);
            //===============Legend==============//
            Legend legend = chart.Legend;
            //AssertHelper.AreEqual(true, legend.Border.isAuto, &quot;&quot;);
            AssertHelper.AreEqual(FormattingType.Automatic, legend.Area.Formatting, &quot;legend.Area.Formatting&quot;);
            ReflectInvoker.invoke(&quot;legend&quot;, legend, new Object[][]{
			    new Object[] {&quot;Shadow&quot;, false},
                new Object[] {&quot;AutoScaleFont&quot;, false},
                new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic},
                new Object[] {&quot;Position&quot;, LegendPositionType.Right}
              });
            font = legend.TextFont;
            ReflectInvoker.invoke(&quot;legend.TextFont&quot;, font, new Object[][]{
			    new Object[] {&quot;Name&quot;, &quot;Tahoma&quot;},
                new Object[] {&quot;Size&quot;, 10},
                new Object[] {&quot;Underline&quot;, FontUnderlineType.None},
                new Object[] {&quot;IsBold&quot;, false},
                new Object[] {&quot;IsItalic&quot;, false},
                new Object[] {&quot;IsStrikeout&quot;, false},
                new Object[] {&quot;IsSubscript&quot;, false},
                new Object[] {&quot;IsSuperscript&quot;, false}
             });
            //===================NSeries=================//
            SeriesCollection nseries = chart.NSeries;
            ReflectInvoker.invoke(&quot;nseries&quot;, nseries, new Object[][]{
			    new Object[] {&quot;CategoryData&quot;, &quot;=Data!$A$2:$A$8&quot;},
                new Object[] {&quot;IsColorVaried&quot;, true}
             });
            //==================ASeries==================//
            Series aseries = nseries[0];
            //AssertHelper.AreEqual(true, aseries.Line.IsAuto, &quot;&quot;);
            //CELLSNET-54095
            ReflectInvoker.invoke(&quot;aseries&quot;, aseries, new Object[][]{
                 new Object[] {&quot;Shadow&quot;, false},
                 new Object[] {&quot;SplitType&quot;, ChartSplitType.Position},
                 //new Object[] {&quot;SplitValue&quot;, 3.0},
                 new Object[] {&quot;IsAutoSplit&quot;, true},
                 new Object[] {&quot;SecondPlotSize&quot;, (short)75},
                 new Object[] {&quot;HasSeriesLines&quot;, true},
                 new Object[] {&quot;IsColorVaried&quot;, true},
                 new Object[] {&quot;GapWidth&quot;, (short)100}
               });
            //=============DataLabels======================//
            DataLabels datalabels = aseries.DataLabels;
            ReflectInvoker.invoke(&quot;datalabels&quot;, datalabels, new Object[][]{
                new Object[] { &quot;ShowSeriesName&quot;, false},
                new Object[] { &quot;ShowCategoryName&quot;, false},
                new Object[] { &quot;ShowValue&quot;, true},
                new Object[] { &quot;ShowPercentage&quot;, false},
                new Object[] {&quot;Separator&quot;, DataLabelsSeparatorType.Auto},
                new Object[] { &quot;ShowLegendKey&quot;, false},
                new Object[] {&quot;Shadow&quot;, false},
                new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic},
                new Object[] {&quot;NumberFormatLinked&quot;, true},
                new Object[] {&quot;TextHorizontalAlignment&quot;, TextAlignmentType.Center},
                new Object[] {&quot;TextVerticalAlignment&quot;, TextAlignmentType.Center},
                new Object[] {&quot;TextDirection&quot;, TextDirectionType.Context},
                new Object[] { &quot;RotationAngle&quot;, 0}
             });
            font = datalabels.TextFont;
            ReflectInvoker.invoke(&quot;datalabels.TextFont&quot;, font, new Object[][]{
                new Object[] {&quot;Name&quot;, &quot;Tahoma&quot;},
                new Object[] {&quot;Size&quot;, 10},
                new Object[] {&quot;Underline&quot;, FontUnderlineType.None},
                new Object[] {&quot;IsBold&quot;, false},
                new Object[] {&quot;IsItalic&quot;, false},
                new Object[] {&quot;IsStrikeout&quot;, false},
                new Object[] {&quot;IsSubscript&quot;, false},
                new Object[] {&quot;IsSuperscript&quot;, false}
             }); 
        }
```

### See Also

* class [Area](../../../aspose.cells.drawing/area/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


