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
// Called: ReflectInvoker.invoke(&amp;quot;categoryaxis.AxisLine&amp;quot;, categoryaxis.AxisLine, new Object[][]{
[Test]
        public void Property_AxisLine()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Charts\\ClusteredColumn.xls&quot;);
            Worksheet worksheet = workbook.Worksheets[0];
            Chart chart = worksheet.Charts[0];
            ReflectInvoker.invoke(&quot;chart&quot;, chart, new Object[][]{
		        new Object[]{&quot;Type&quot;, ChartType.Column},
                new Object[] {&quot;IsRectangularCornered&quot;, true},
                new Object[] { &quot;ShowLegend&quot;, true},
                new Object[] { &quot;ShowDataTable&quot;, false}});
            ReflectInvoker.invoke(&quot;chart.ChartObject&quot;, chart.ChartObject, new Object[][]{
                new Object[] { &quot;IsPrintable&quot;, true},
			    new Object[]{&quot;IsLocked&quot;, true},
                new Object[] {&quot;Placement&quot;, PlacementType.Move}});
            //================ChartArea=====================//
            ChartArea chartArea = chart.ChartArea;
            //AssertHelper.AreEqual(true, chartArea.Border.IsAuto, &quot;&quot;);
            AssertHelper.AreEqual(FormattingType.Automatic, chartArea.Area.Formatting, &quot;chartArea.Area.Formatting&quot;);
            ReflectInvoker.invoke(&quot;chartArea&quot;, chartArea, new Object[][]{
                new Object[]{&quot;Shadow&quot;, true},
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
            //===============ChartTitle=======================//           
            Title title = chart.Title;
            AssertHelper.AreEqual(false, title.Border.IsVisible, &quot;title.Border.IsVisible&quot;);
            AssertHelper.AreEqual(FormattingType.None, title.Area.Formatting, &quot;title.Area.Formatting&quot;);
            ReflectInvoker.invoke(&quot;title&quot;, title, new Object[][]{
                new Object[] {&quot;Text&quot;, &quot;Marketing Costs by Region&quot;},
                new Object[] {&quot;Shadow&quot;, true},
                new Object[] {&quot;AutoScaleFont&quot;, false},
                new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic},
                new Object[] {&quot;TextHorizontalAlignment&quot;, TextAlignmentType.Center},
                new Object[] {&quot;TextVerticalAlignment&quot;, TextAlignmentType.Center},
                new Object[] {&quot;TextDirection&quot;,TextDirectionType.Context},
                new Object[] { &quot;RotationAngle&quot;, 0}});

            ReflectInvoker.invoke(&quot;title.TextFont&quot;, title.Font, new Object[][]{
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
            //=================legend========================//
            Legend legend = chart.Legend;
            ReflectInvoker.invoke(&quot;legend.Border&quot;, legend.Border, new Object[][]{
            new Object[] {&quot;Color&quot;, Color.Red},
            new Object[] {&quot;Style&quot;, LineType.MediumGray},
            new Object[] {&quot;Weight&quot;, WeightType.MediumLine}});
            //Assert.AreEqual(FormatSetType.IsTextureSet, legend.Area.FillFormat.SetType, &quot;legend.Area.FillFormat.SetType&quot;);
            Assert.AreEqual(TextureType.RecycledPaper, legend.Area.FillFormat.Texture, &quot;legend.Area.FillFormat.Texture&quot;);

            ReflectInvoker.invoke(&quot;legend&quot;, legend, new Object[][]{
                new Object[] {&quot;Shadow&quot;, true},
                new Object[] {&quot;AutoScaleFont&quot;, false},
                new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic},
                new Object[] {&quot;Position&quot;, LegendPositionType.Top}});

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
            //=================PlotArea=======================//           
            ReflectInvoker.invoke(&quot;chart.PlotArea.Border&quot;, chart.PlotArea.Border, new Object[][]{
            new Object[] {&quot;Color&quot;, Color.Empty},
            new Object[] {&quot;Style&quot;, LineType.Solid},
            new Object[] {&quot;Weight&quot;, WeightType.HairLine}});
            AssertHelper.AreEqual(FormattingType.Automatic, chart.PlotArea.Area.Formatting, &quot;chart.PlotArea.Area.Formatting&quot;);
            //================CategoryAxis=====================//
            Axis categoryaxis = chart.CategoryAxis;
            AssertHelper.AreEqual(false, categoryaxis.MajorGridLines.IsVisible, &quot;categoryaxis.MajorGridLines.IsVisible&quot;);
            AssertHelper.AreEqual(false, categoryaxis.MinorGridLines.IsVisible, &quot;categoryaxis.MinorGridLines.IsVisible&quot;);

            ReflectInvoker.invoke(&quot;categoryaxis.AxisLine&quot;, categoryaxis.AxisLine, new Object[][]{
                new Object[] {&quot;Color&quot;, Color.Empty},
                new Object[] {&quot;Style&quot;, LineType.Solid},
                new Object[] {&quot;Weight&quot;, WeightType.HairLine}});
            ReflectInvoker.invoke(&quot;categoryaxis&quot;, categoryaxis, new Object[][]{
                new Object[] {&quot;MajorTickMark&quot;, TickMarkType.Inside},
                new Object[] {&quot;MinorTickMark&quot;, TickMarkType.None},
                new Object[] {&quot;TickLabelPosition&quot;, TickLabelPositionType.NextToAxis},
                new Object[] {&quot;TickLabelSpacing&quot;, 2},
                new Object[] {&quot;TickMarkSpacing&quot;, 3},
                new Object[] {&quot;AxisBetweenCategories&quot;, true},
                new Object[] {&quot;IsPlotOrderReversed&quot;, false},
                //new Object[] {&quot;isCrossAtMax&quot;, false},
                new Object[] {&quot;IsVisible&quot;, true},
                new Object[] {&quot;CategoryType&quot;, CategoryType.AutomaticScale}
            });
            ReflectInvoker.invoke(&quot;categoryaxis.TickLabels&quot;, categoryaxis.TickLabels, new Object[][]{
                new Object[]{&quot;AutoScaleFont&quot;, false},
                new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Transparent},
                new Object[] {&quot;NumberFormatLinked&quot;, true},
                new Object[] { &quot;RotationAngle&quot;, 0},
                new Object[] {&quot;Offset&quot;, 100},
                new Object[] {&quot;TextDirection&quot;, TextDirectionType.Context}});

            ReflectInvoker.invoke(&quot;categoryaxis.TickLabels.Font&quot;, categoryaxis.TickLabels.Font, new Object[][]{
                new Object[]{&quot;Name&quot;, FontNameConstants.zh_SongTi},
                new Object[]{&quot;Size&quot;, 10},
                new Object[]{&quot;Underline&quot;, FontUnderlineType.None},
                new Object[]{&quot;Color&quot;, Color.Red},
                new Object[]{&quot;IsBold&quot;, false},
                new Object[]{&quot;IsItalic&quot;, false},
                new Object[]{&quot;IsStrikeout&quot;, false},
                new Object[]{&quot;IsSubscript&quot;, false},
                new Object[]{&quot;IsSuperscript&quot;, false}});

            Title categoryTitle = categoryaxis.Title;
            AssertHelper.AreEqual(false, categoryTitle.Border.IsVisible, &quot;categoryaxis.Title.Border.IsVisible&quot;);
            AssertHelper.AreEqual(FormattingType.Automatic, categoryTitle.Area.Formatting, &quot;categoryTitle.Area.Formatting&quot;);
            ReflectInvoker.invoke(&quot;categoryaxis.Title&quot;, categoryTitle, new Object[][]{
                new Object[]{&quot;Text&quot;, &quot;Region&quot;},
                new Object[] {&quot;Shadow&quot;, false},
                new Object[] {&quot;AutoScaleFont&quot;, false},
                new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Transparent},
                new Object[]{&quot;TextHorizontalAlignment&quot;,TextAlignmentType.Right},
                new Object[]{&quot;TextVerticalAlignment&quot;,TextAlignmentType.Bottom},
                new Object[]{&quot;TextDirection&quot;,TextDirectionType.LeftToRight},
                new Object[]{ &quot;RotationAngle&quot;, -20}});
            ReflectInvoker.invoke(&quot;categoryaxis.getTitle.getFont&quot;, categoryTitle.TextFont, new Object[][]{
                new Object[]{&quot;Name&quot;, &quot;Tahoma&quot;},
                new Object[]{&quot;Size&quot;, 16},
                new Object[]{&quot;Underline&quot;, FontUnderlineType.Single},
                new Object[]{&quot;Color&quot;, Color.Red},
                new Object[]{&quot;IsBold&quot;, false},
                new Object[]{&quot;IsItalic&quot;, false},
                new Object[]{&quot;IsStrikeout&quot;, false},
                new Object[]{&quot;IsSuperscript&quot;, true},
                new Object[] {&quot;IsSubscript&quot;, false}});
            //==================ValueAxis====================//
            Axis valueaxis = chart.ValueAxis;
            AssertHelper.AreEqual(false, valueaxis.MajorGridLines.IsVisible, &quot;valueaxis.MajorGridLines.IsVisible&quot;);
            AssertHelper.AreEqual(false, valueaxis.MinorGridLines.IsVisible, &quot;valueaxis.MinorGridLines.IsVisible&quot;);

            ReflectInvoker.invoke(&quot;valueaxis.AxisLine&quot;, valueaxis.AxisLine, new Object[][]{
                new Object[] {&quot;Color&quot;, Color.Red},
                new Object[] {&quot;Style&quot;, LineType.Solid},
                new Object[] {&quot;Weight&quot;, WeightType.HairLine}});
            ReflectInvoker.invoke(&quot;valueaxis&quot;, valueaxis, new Object[][]{
                new Object[] {&quot;MajorTickMark&quot;, TickMarkType.Inside},
                new Object[] {&quot;MinorTickMark&quot;, TickMarkType.None},
                new Object[] {&quot;TickLabelPosition&quot;, TickLabelPositionType.High},
                new Object[] {&quot;MinValue&quot;, 0d},
                new Object[] {&quot;MaxValue&quot;, 80000d},
                new Object[] {&quot;MajorUnit&quot;, 20000d},
                new Object[] {&quot;MinorUnit&quot;, 5000d},
                new Object[] {&quot;CrossAt&quot;, 10d},
                new Object[] {&quot;IsLogarithmic&quot;, false},
                new Object[] {&quot;IsPlotOrderReversed&quot;, false},
                new Object[] {&quot;IsVisible&quot;, true}
                //new Object[] {&quot;isCrossAtMax&quot;, false},
                });

            ReflectInvoker.invoke(&quot;valueaxis.TickLabels&quot;, valueaxis.TickLabels, new Object[][]{
                 new Object[]{&quot;AutoScaleFont&quot;, false},
                 new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Transparent},
                 new Object[] {&quot;NumberFormatLinked&quot;, false},
                 new Object[] {&quot;NumberFormat&quot;, &quot;\&quot;$\&quot;#,##0&quot;},
                 new Object[] { &quot;RotationAngle&quot;, 30},
                 new Object[] {&quot;TextDirection&quot;, TextDirectionType.Context}
             });

            ReflectInvoker.invoke(&quot;valueaxis.TickLabels.Font&quot;, valueaxis.TickLabels.Font, new Object[][]{
                new Object[]{&quot;Name&quot;, &quot;Tahoma&quot;},
                new Object[]{&quot;Size&quot;, 10},
                new Object[]{&quot;Underline&quot;, FontUnderlineType.None},
                new Object[]{&quot;Color&quot;, Color.Black},
                new Object[]{&quot;IsBold&quot;, true},
                new Object[]{&quot;IsItalic&quot;, false},
                new Object[]{&quot;IsStrikeout&quot;, false},
                new Object[]{&quot;IsSubscript&quot;, false},
                new Object[] {&quot;IsSuperscript&quot;, false}});
            //=====//		
            Title valueTitle = valueaxis.Title;
            AssertHelper.AreEqual(false, valueTitle.Border.IsVisible, &quot;valueaxis.Title.Border.IsVisible&quot;);
            AssertHelper.AreEqual(FormattingType.None, valueTitle.Area.Formatting, &quot;valueaxis.Title.Area.Formatting&quot;);
            ReflectInvoker.invoke(&quot;valueaxis.Title&quot;, valueTitle, new Object[][]{
                new Object[] {&quot;Text&quot;, &quot;In Thousands&quot;},
                new Object[] {&quot;Shadow&quot;, false},
                new Object[] {&quot;AutoScaleFont&quot;, false}, 
                new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic}, 
                new Object[] {&quot;TextHorizontalAlignment&quot;, TextAlignmentType.Center},
                new Object[] {&quot;TextVerticalAlignment&quot;,TextAlignmentType.Center},
                new Object[] { &quot;RotationAngle&quot;, 90},
                new Object[] {&quot;TextDirection&quot;, TextDirectionType.Context}});

            ReflectInvoker.invoke(&quot;valueaxis.Title.TextFont&quot;, valueaxis.Title.TextFont, new Object[][]{
                new Object[]{&quot;Name&quot;, &quot;Tahoma&quot;},
                new Object[]{&quot;Size&quot;, 12},
                new Object[]{&quot;Underline&quot;, FontUnderlineType.None},
                new Object[]{&quot;Color&quot;, Color.Black},
                new Object[]{&quot;IsBold&quot;, false},
                new Object[]{&quot;IsItalic&quot;, false},
                new Object[]{&quot;IsStrikeout&quot;, true},
                new Object[]{&quot;IsSubscript&quot;, false}, 
                new Object[] {&quot;IsSuperscript&quot;, false}});
            //==============DisplayUnitLabel==================//
            DisplayUnitLabel displayunitlabel = valueaxis.DisplayUnitLabel;
            AssertHelper.AreEqual(false, displayunitlabel.Border.IsVisible, &quot;displayunitlabel.Border.IsVisible&quot;);
            AssertHelper.AreEqual(FormattingType.None, displayunitlabel.Area.Formatting, &quot;displayunitlabel.Area.Formatting&quot;);
            ReflectInvoker.invoke(&quot;displayunitlabel&quot;, displayunitlabel, new Object[][]{
                new Object[] {&quot;Text&quot;, &quot;Thousands&quot;},
                new Object[] {&quot;Shadow&quot;, false},
                new Object[] {&quot;AutoScaleFont&quot;, true},
                new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic},
                new Object[] {&quot;TextHorizontalAlignment&quot;, TextAlignmentType.Center},
                new Object[] {&quot;TextVerticalAlignment&quot;, TextAlignmentType.Center},
                new Object[] {&quot;TextDirection&quot;, TextDirectionType.Context},
                new Object[] { &quot;RotationAngle&quot;, 90}
            });
            //CELLSNET - 54093
            ReflectInvoker.invoke(&quot;displayunitlabel.TextFont&quot;, displayunitlabel.TextFont, new Object[][]{
                new Object[]{&quot;Name&quot;, &quot;Tahoma&quot;},
                //new Object[]{&quot;Size&quot;, 9},
                new Object[]{&quot;Underline&quot;, FontUnderlineType.None},
                new Object[]{&quot;Color&quot;, Color.Red},
                new Object[]{&quot;IsBold&quot;, true},
                new Object[]{&quot;IsItalic&quot;, false},
                new Object[]{&quot;IsStrikeout&quot;, false},
                new Object[]{&quot;IsSubscript&quot;, false},
                new Object[]{&quot;IsSuperscript&quot;, false}});
            //===========================NSeries====================//
            SeriesCollection nseries = chart.NSeries;
            ReflectInvoker.invoke(&quot;nseries&quot;, nseries, new Object[][]{
                new Object[] {&quot;CategoryData&quot;,&quot;=&apos;Clustered Column&apos;!$A$2:$A$4&quot;},
                new Object[] {&quot;Count&quot;, 1}});
            //==========================ASeries===================//
            Series aseries = nseries[0];
            //AssertHelper.AreEqual(true, aseries.Line.IsAuto, &quot;aseries.Line.IsAuto&quot;);
            AssertHelper.AreEqual(FormattingType.Automatic, aseries.Area.Formatting, &quot;aseries.Area.Formatting&quot;);
            ReflectInvoker.invoke(&quot;aseries&quot;, aseries, new Object[][]{		
                new Object[] {&quot;Shadow&quot;, false}, 
                new Object[] {&quot;Overlap&quot;, (short)0},
                new Object[] {&quot;GapWidth&quot;, (short)80},
                new Object[] {&quot;IsColorVaried&quot;, true}});
            //=========================YErroBars================//
            ErrorBar yErrorbar = aseries.YErrorBar;
            ReflectInvoker.invoke(&quot;yErrorbar&quot;, yErrorbar, new Object[][]{
                new Object[] {&quot;DisplayType&quot;, ErrorBarDisplayType.Minus},
                 new Object[] {&quot;Type&quot;, ErrorBarType.Percent}, 
                new Object[] {&quot;Amount&quot;, 5d}       
                });
            //========================DataLabels===============//
            DataLabels datalabels = aseries.DataLabels;
            ReflectInvoker.invoke(&quot;datalabels&quot;, datalabels, new Object[][]{
                new Object[] { &quot;ShowSeriesName&quot;, false},
                new Object[] { &quot;ShowCategoryName&quot;, true},
                new Object[] { &quot;ShowValue&quot;, true},
                new Object[] {&quot;Separator&quot;, DataLabelsSeparatorType.Comma},
                new Object[] { &quot;ShowLegendKey&quot;, false}, 
                new Object[] {&quot;Shadow&quot;, false},
                 new Object[] {&quot;AutoScaleFont&quot;, false},
                new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic},
                new Object[] {&quot;NumberFormatLinked&quot;, false},
                new Object[] {&quot;NumberFormat&quot;, &quot;\&quot;$\&quot;#,##0&quot;},
                new Object[] {&quot;TextHorizontalAlignment&quot;, TextAlignmentType.Center},
                new Object[] {&quot;TextVerticalAlignment&quot;, TextAlignmentType.Center},
                new Object[] {&quot;Position&quot;, LabelPositionType.OutsideEnd},
                new Object[] {&quot;TextDirection&quot;, TextDirectionType.Context},
                new Object[] { &quot;RotationAngle&quot;, 0}
             });
            AssertHelper.AreEqual(false, datalabels.Border.IsVisible, &quot;datalabels.Border.IsVisible&quot;);
            AssertHelper.AreEqual(FormattingType.None, datalabels.Area.Formatting, &quot;datalabels.Area.Formatting&quot;);

            ReflectInvoker.invoke(&quot;datalabels.TextFont&quot;, datalabels.TextFont, new Object[][]{
                new Object[]{&quot;Name&quot;, &quot;Tahoma&quot;},
                new Object[]{&quot;Size&quot;, 10},
                new Object[]{&quot;Underline&quot;, FontUnderlineType.None},
                new Object[]{&quot;Color&quot;, Color.Black},
                new Object[]{&quot;IsBold&quot;, true},
                new Object[]{&quot;IsItalic&quot;, false},
                new Object[]{&quot;IsStrikeout&quot;, false},
                new Object[]{&quot;IsSubscript&quot;, false},
                new Object[]{&quot;IsSuperscript&quot;, false}});          
        }
```

### See Also

* class [Line](../../../aspose.cells.drawing/line/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


