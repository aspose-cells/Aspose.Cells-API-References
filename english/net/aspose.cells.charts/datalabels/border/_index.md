---
title: DataLabels.Border
second_title: Aspose.Cells for .NET API Reference
description: DataLabels property. Gets the border
type: docs
url: /net/aspose.cells.charts/datalabels/border/
---
## DataLabels.Border property

Gets the [`border`](../../../aspose.cells.drawing/line/).

```csharp
public override Line Border { get; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(false, datalabels.Border.IsVisible, "datalabels.Border.IsVisible");
[Test]
        public void Property_Border()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "Charts\\ClusteredColumn.xls");
            Worksheet worksheet = workbook.Worksheets[0];
            Chart chart = worksheet.Charts[0];
            ReflectInvoker.invoke("chart", chart, new Object[][]{
		        new Object[]{"Type", ChartType.Column},
                new Object[] {"IsRectangularCornered", true},
                new Object[] { "ShowLegend", true},
                new Object[] { "ShowDataTable", false}});
            ReflectInvoker.invoke("chart.ChartObject", chart.ChartObject, new Object[][]{
                new Object[] { "IsPrintable", true},
			    new Object[]{"IsLocked", true},
                new Object[] {"Placement", PlacementType.Move}});
            //================ChartArea=====================//
            ChartArea chartArea = chart.ChartArea;
            //AssertHelper.AreEqual(true, chartArea.Border.IsAuto, "");
            AssertHelper.AreEqual(FormattingType.Automatic, chartArea.Area.Formatting, "chartArea.Area.Formatting");
            ReflectInvoker.invoke("chartArea", chartArea, new Object[][]{
                new Object[]{"Shadow", true},
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
            //===============ChartTitle=======================//           
            Title title = chart.Title;
            AssertHelper.AreEqual(false, title.Border.IsVisible, "title.Border.IsVisible");
            AssertHelper.AreEqual(FormattingType.None, title.Area.Formatting, "title.Area.Formatting");
            ReflectInvoker.invoke("title", title, new Object[][]{
                new Object[] {"Text", "Marketing Costs by Region"},
                new Object[] {"Shadow", true},
                new Object[] {"AutoScaleFont", false},
                new Object[] { "BackgroundMode", BackgroundMode.Automatic},
                new Object[] {"TextHorizontalAlignment", TextAlignmentType.Center},
                new Object[] {"TextVerticalAlignment", TextAlignmentType.Center},
                new Object[] {"TextDirection",TextDirectionType.Context},
                new Object[] { "RotationAngle", 0}});

            ReflectInvoker.invoke("title.TextFont", title.Font, new Object[][]{
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
            //=================legend========================//
            Legend legend = chart.Legend;
            ReflectInvoker.invoke("legend.Border", legend.Border, new Object[][]{
            new Object[] {"Color", Color.Red},
            new Object[] {"Style", LineType.MediumGray},
            new Object[] {"Weight", WeightType.MediumLine}});
            //Assert.AreEqual(FormatSetType.IsTextureSet, legend.Area.FillFormat.SetType, "legend.Area.FillFormat.SetType");
            Assert.AreEqual(TextureType.RecycledPaper, legend.Area.FillFormat.Texture, "legend.Area.FillFormat.Texture");

            ReflectInvoker.invoke("legend", legend, new Object[][]{
                new Object[] {"Shadow", true},
                new Object[] {"AutoScaleFont", false},
                new Object[] { "BackgroundMode", BackgroundMode.Automatic},
                new Object[] {"Position", LegendPositionType.Top}});

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
            //=================PlotArea=======================//           
            ReflectInvoker.invoke("chart.PlotArea.Border", chart.PlotArea.Border, new Object[][]{
            new Object[] {"Color", Color.Empty},
            new Object[] {"Style", LineType.Solid},
            new Object[] {"Weight", WeightType.HairLine}});
            AssertHelper.AreEqual(FormattingType.Automatic, chart.PlotArea.Area.Formatting, "chart.PlotArea.Area.Formatting");
            //================CategoryAxis=====================//
            Axis categoryaxis = chart.CategoryAxis;
            AssertHelper.AreEqual(false, categoryaxis.MajorGridLines.IsVisible, "categoryaxis.MajorGridLines.IsVisible");
            AssertHelper.AreEqual(false, categoryaxis.MinorGridLines.IsVisible, "categoryaxis.MinorGridLines.IsVisible");

            ReflectInvoker.invoke("categoryaxis.AxisLine", categoryaxis.AxisLine, new Object[][]{
                new Object[] {"Color", Color.Empty},
                new Object[] {"Style", LineType.Solid},
                new Object[] {"Weight", WeightType.HairLine}});
            ReflectInvoker.invoke("categoryaxis", categoryaxis, new Object[][]{
                new Object[] {"MajorTickMark", TickMarkType.Inside},
                new Object[] {"MinorTickMark", TickMarkType.None},
                new Object[] {"TickLabelPosition", TickLabelPositionType.NextToAxis},
                new Object[] {"TickLabelSpacing", 2},
                new Object[] {"TickMarkSpacing", 3},
                new Object[] {"AxisBetweenCategories", true},
                new Object[] {"IsPlotOrderReversed", false},
                //new Object[] {"isCrossAtMax", false},
                new Object[] {"IsVisible", true},
                new Object[] {"CategoryType", CategoryType.AutomaticScale}
            });
            ReflectInvoker.invoke("categoryaxis.TickLabels", categoryaxis.TickLabels, new Object[][]{
                new Object[]{"AutoScaleFont", false},
                new Object[] { "BackgroundMode", BackgroundMode.Transparent},
                new Object[] {"NumberFormatLinked", true},
                new Object[] { "RotationAngle", 0},
                new Object[] {"Offset", 100},
                new Object[] {"TextDirection", TextDirectionType.Context}});

            ReflectInvoker.invoke("categoryaxis.TickLabels.Font", categoryaxis.TickLabels.Font, new Object[][]{
                new Object[]{"Name", FontNameConstants.zh_SongTi},
                new Object[]{"Size", 10},
                new Object[]{"Underline", FontUnderlineType.None},
                new Object[]{"Color", Color.Red},
                new Object[]{"IsBold", false},
                new Object[]{"IsItalic", false},
                new Object[]{"IsStrikeout", false},
                new Object[]{"IsSubscript", false},
                new Object[]{"IsSuperscript", false}});

            Title categoryTitle = categoryaxis.Title;
            AssertHelper.AreEqual(false, categoryTitle.Border.IsVisible, "categoryaxis.Title.Border.IsVisible");
            AssertHelper.AreEqual(FormattingType.Automatic, categoryTitle.Area.Formatting, "categoryTitle.Area.Formatting");
            ReflectInvoker.invoke("categoryaxis.Title", categoryTitle, new Object[][]{
                new Object[]{"Text", "Region"},
                new Object[] {"Shadow", false},
                new Object[] {"AutoScaleFont", false},
                new Object[] { "BackgroundMode", BackgroundMode.Transparent},
                new Object[]{"TextHorizontalAlignment",TextAlignmentType.Right},
                new Object[]{"TextVerticalAlignment",TextAlignmentType.Bottom},
                new Object[]{"TextDirection",TextDirectionType.LeftToRight},
                new Object[]{ "RotationAngle", -20}});
            ReflectInvoker.invoke("categoryaxis.getTitle.getFont", categoryTitle.TextFont, new Object[][]{
                new Object[]{"Name", "Tahoma"},
                new Object[]{"Size", 16},
                new Object[]{"Underline", FontUnderlineType.Single},
                new Object[]{"Color", Color.Red},
                new Object[]{"IsBold", false},
                new Object[]{"IsItalic", false},
                new Object[]{"IsStrikeout", false},
                new Object[]{"IsSuperscript", true},
                new Object[] {"IsSubscript", false}});
            //==================ValueAxis====================//
            Axis valueaxis = chart.ValueAxis;
            AssertHelper.AreEqual(false, valueaxis.MajorGridLines.IsVisible, "valueaxis.MajorGridLines.IsVisible");
            AssertHelper.AreEqual(false, valueaxis.MinorGridLines.IsVisible, "valueaxis.MinorGridLines.IsVisible");

            ReflectInvoker.invoke("valueaxis.AxisLine", valueaxis.AxisLine, new Object[][]{
                new Object[] {"Color", Color.Red},
                new Object[] {"Style", LineType.Solid},
                new Object[] {"Weight", WeightType.HairLine}});
            ReflectInvoker.invoke("valueaxis", valueaxis, new Object[][]{
                new Object[] {"MajorTickMark", TickMarkType.Inside},
                new Object[] {"MinorTickMark", TickMarkType.None},
                new Object[] {"TickLabelPosition", TickLabelPositionType.High},
                new Object[] {"MinValue", 0d},
                new Object[] {"MaxValue", 80000d},
                new Object[] {"MajorUnit", 20000d},
                new Object[] {"MinorUnit", 5000d},
                new Object[] {"CrossAt", 10d},
                new Object[] {"IsLogarithmic", false},
                new Object[] {"IsPlotOrderReversed", false},
                new Object[] {"IsVisible", true}
                //new Object[] {"isCrossAtMax", false},
                });

            ReflectInvoker.invoke("valueaxis.TickLabels", valueaxis.TickLabels, new Object[][]{
                 new Object[]{"AutoScaleFont", false},
                 new Object[] { "BackgroundMode", BackgroundMode.Transparent},
                 new Object[] {"NumberFormatLinked", false},
                 new Object[] {"NumberFormat", "\"$\"#,##0"},
                 new Object[] { "RotationAngle", 30},
                 new Object[] {"TextDirection", TextDirectionType.Context}
             });

            ReflectInvoker.invoke("valueaxis.TickLabels.Font", valueaxis.TickLabels.Font, new Object[][]{
                new Object[]{"Name", "Tahoma"},
                new Object[]{"Size", 10},
                new Object[]{"Underline", FontUnderlineType.None},
                new Object[]{"Color", Color.Black},
                new Object[]{"IsBold", true},
                new Object[]{"IsItalic", false},
                new Object[]{"IsStrikeout", false},
                new Object[]{"IsSubscript", false},
                new Object[] {"IsSuperscript", false}});
            //=====//		
            Title valueTitle = valueaxis.Title;
            AssertHelper.AreEqual(false, valueTitle.Border.IsVisible, "valueaxis.Title.Border.IsVisible");
            AssertHelper.AreEqual(FormattingType.None, valueTitle.Area.Formatting, "valueaxis.Title.Area.Formatting");
            ReflectInvoker.invoke("valueaxis.Title", valueTitle, new Object[][]{
                new Object[] {"Text", "In Thousands"},
                new Object[] {"Shadow", false},
                new Object[] {"AutoScaleFont", false}, 
                new Object[] { "BackgroundMode", BackgroundMode.Automatic}, 
                new Object[] {"TextHorizontalAlignment", TextAlignmentType.Center},
                new Object[] {"TextVerticalAlignment",TextAlignmentType.Center},
                new Object[] { "RotationAngle", 90},
                new Object[] {"TextDirection", TextDirectionType.Context}});

            ReflectInvoker.invoke("valueaxis.Title.TextFont", valueaxis.Title.TextFont, new Object[][]{
                new Object[]{"Name", "Tahoma"},
                new Object[]{"Size", 12},
                new Object[]{"Underline", FontUnderlineType.None},
                new Object[]{"Color", Color.Black},
                new Object[]{"IsBold", false},
                new Object[]{"IsItalic", false},
                new Object[]{"IsStrikeout", true},
                new Object[]{"IsSubscript", false}, 
                new Object[] {"IsSuperscript", false}});
            //==============DisplayUnitLabel==================//
            DisplayUnitLabel displayunitlabel = valueaxis.DisplayUnitLabel;
            AssertHelper.AreEqual(false, displayunitlabel.Border.IsVisible, "displayunitlabel.Border.IsVisible");
            AssertHelper.AreEqual(FormattingType.None, displayunitlabel.Area.Formatting, "displayunitlabel.Area.Formatting");
            ReflectInvoker.invoke("displayunitlabel", displayunitlabel, new Object[][]{
                new Object[] {"Text", "Thousands"},
                new Object[] {"Shadow", false},
                new Object[] {"AutoScaleFont", true},
                new Object[] { "BackgroundMode", BackgroundMode.Automatic},
                new Object[] {"TextHorizontalAlignment", TextAlignmentType.Center},
                new Object[] {"TextVerticalAlignment", TextAlignmentType.Center},
                new Object[] {"TextDirection", TextDirectionType.Context},
                new Object[] { "RotationAngle", 90}
            });
            //CELLSNET - 54093
            ReflectInvoker.invoke("displayunitlabel.TextFont", displayunitlabel.TextFont, new Object[][]{
                new Object[]{"Name", "Tahoma"},
                //new Object[]{"Size", 9},
                new Object[]{"Underline", FontUnderlineType.None},
                new Object[]{"Color", Color.Red},
                new Object[]{"IsBold", true},
                new Object[]{"IsItalic", false},
                new Object[]{"IsStrikeout", false},
                new Object[]{"IsSubscript", false},
                new Object[]{"IsSuperscript", false}});
            //===========================NSeries====================//
            SeriesCollection nseries = chart.NSeries;
            ReflectInvoker.invoke("nseries", nseries, new Object[][]{
                new Object[] {"CategoryData","='Clustered Column'!$A$2:$A$4"},
                new Object[] {"Count", 1}});
            //==========================ASeries===================//
            Series aseries = nseries[0];
            //AssertHelper.AreEqual(true, aseries.Line.IsAuto, "aseries.Line.IsAuto");
            AssertHelper.AreEqual(FormattingType.Automatic, aseries.Area.Formatting, "aseries.Area.Formatting");
            ReflectInvoker.invoke("aseries", aseries, new Object[][]{		
                new Object[] {"Shadow", false}, 
                new Object[] {"Overlap", (short)0},
                new Object[] {"GapWidth", (short)80},
                new Object[] {"IsColorVaried", true}});
            //=========================YErroBars================//
            ErrorBar yErrorbar = aseries.YErrorBar;
            ReflectInvoker.invoke("yErrorbar", yErrorbar, new Object[][]{
                new Object[] {"DisplayType", ErrorBarDisplayType.Minus},
                 new Object[] {"Type", ErrorBarType.Percent}, 
                new Object[] {"Amount", 5d}       
                });
            //========================DataLabels===============//
            DataLabels datalabels = aseries.DataLabels;
            ReflectInvoker.invoke("datalabels", datalabels, new Object[][]{
                new Object[] { "ShowSeriesName", false},
                new Object[] { "ShowCategoryName", true},
                new Object[] { "ShowValue", true},
                new Object[] {"Separator", DataLabelsSeparatorType.Comma},
                new Object[] { "ShowLegendKey", false}, 
                new Object[] {"Shadow", false},
                 new Object[] {"AutoScaleFont", false},
                new Object[] { "BackgroundMode", BackgroundMode.Automatic},
                new Object[] {"NumberFormatLinked", false},
                new Object[] {"NumberFormat", "\"$\"#,##0"},
                new Object[] {"TextHorizontalAlignment", TextAlignmentType.Center},
                new Object[] {"TextVerticalAlignment", TextAlignmentType.Center},
                new Object[] {"Position", LabelPositionType.OutsideEnd},
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
                new Object[]{"IsBold", true},
                new Object[]{"IsItalic", false},
                new Object[]{"IsStrikeout", false},
                new Object[]{"IsSubscript", false},
                new Object[]{"IsSuperscript", false}});          
        }
```

### See Also

* class [Line](../../../aspose.cells.drawing/line/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


