---
title: LegendEntry.TextFont
second_title: Aspose.Cells for .NET API Reference
description: LegendEntry property. Gets a Font object of the specified LegendEntry object
type: docs
url: /net/aspose.cells.charts/legendentry/textfont/
---
## LegendEntry.TextFont property

Gets a [`Font`](../font/) object of the specified LegendEntry object.

```csharp
[Obsolete("Use LegendEntry.Font property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual Font TextFont { get; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use LegendEntry.Font property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: ReflectInvoker.invoke("legendEntry3.TextFont", legendEntry3.TextFont, new Object[][]{
[Test]
        public void Property_TextFont()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "Charts\\Contour.xls");
            Worksheet worksheet = workbook.Worksheets[0];
            Chart chart = worksheet.Charts[0];
            ReflectInvoker.invoke("chart", chart, new Object[][]{
			new Object[]{"Type", ChartType.SurfaceContour},
            new Object[] {"IsRectangularCornered", true},
            new Object[] { "ShowLegend", true}});  
     
            ReflectInvoker.invoke("chart.ChartObject", chart.ChartObject, new Object[][]{
                new Object[] { "IsPrintable", true},
			    new Object[]{"IsLocked", true},
                new Object[] {"Placement", PlacementType.Move}});
            //===============ChartArea==================//
            ChartArea chartArea = chart.ChartArea;
            //AssertHelper.assertEquals("chartArea.getBorder.isAuto", true, chartArea.getBorder().isAuto());
            AssertHelper.AreEqual(FormattingType.Automatic, chartArea.Area.Formatting, "chartArea.getArea.isAuto");
            ReflectInvoker.invoke("chartArea", chartArea, new Object[][]{
				new Object[]{"Shadow", false},
				new Object[]{"AutoScaleFont", false},
				new Object[] { "BackgroundMode", BackgroundMode.Automatic},
			});               
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
            //===============Title=======================//
            Title title = chart.Title;
            AssertHelper.AreEqual(false, title.Border.IsVisible, "title.Border.IsVisible");
            AssertHelper.AreEqual(FormattingType.None, title.Area.Formatting, "title.Area.Formatting");
            ReflectInvoker.invoke("title", title, new Object[][]{                
				new Object[] {"Text", "Tensile strenth Measurements"},
                new Object[] {"Shadow", false},
                new Object[] {"AutoScaleFont", false},
                new Object[] { "BackgroundMode", BackgroundMode.Automatic},
				new Object[]{"TextHorizontalAlignment", TextAlignmentType.Center},
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
            //=====================Legend========================//
            Legend legend = chart.Legend;
            //AssertHelper.assertEquals("legend.getBorder.isAuto", true, legend.getBorder().isAuto());
            AssertHelper.AreEqual(FormattingType.Automatic, legend.Area.Formatting, "legend.Area.Formatting");
            ReflectInvoker.invoke("legend", legend, new Object[][]{
                new Object[] {"Shadow", false},
				new Object[]{"Position", LegendPositionType.Right},
			});
            //=====================LegendEntry============//
            AssertHelper.AreEqual(5, legend.LegendEntries.Count, "legend.LegendEntries.Count");
            LegendEntryCollection legendEntries = legend.LegendEntries;
            LegendEntry legendEntry1 = legendEntries[0];
            ReflectInvoker.invoke("legendEntry1", legendEntry1, new Object[][]{
                new Object[] {"AutoScaleFont", true},
                new Object[] { "BackgroundMode", BackgroundMode.Automatic},
               });
            ReflectInvoker.invoke("legendEntry1.TextFont", legendEntry1.TextFont, new Object[][]{
			    new Object[]{"Name", "Tahoma"},
			    new Object[]{"Size", 10},
			    new Object[]{"Underline", FontUnderlineType.None},
			    new Object[]{"Color", Color.Red},
			    new Object[]{"IsBold", false},
			    new Object[]{"IsItalic", false},
			    new Object[]{"IsStrikeout", false},
			    new Object[]{"IsSubscript", false},
                new Object[] {"IsSuperscript", false}
			});

            LegendEntry legendEntry2 = legendEntries[1];
            ReflectInvoker.invoke("legendEntry2", legendEntry2, new Object[][]{
                new Object[] {"AutoScaleFont", false},
                new Object[] { "BackgroundMode", BackgroundMode.Automatic},
               });
            ReflectInvoker.invoke("legendEntry2.TextFont", legendEntry2.TextFont, new Object[][]{
			    new Object[]{"Name", FontNameConstants.zh_HeiTi},
			    new Object[]{"Size", 12},
			    new Object[]{"Underline", FontUnderlineType.None},
			    new Object[]{"Color", Color.Black},
			    new Object[]{"IsBold", true},
			    new Object[]{"IsItalic", false},
			    new Object[]{"IsStrikeout", false},
			    new Object[]{"IsSubscript", false},
                new Object[] {"IsSuperscript", false}
			});

            LegendEntry legendEntry3 = legendEntries[2];
            ReflectInvoker.invoke("legendEntry3", legendEntry3, new Object[][]{
                new Object[] {"AutoScaleFont", false},
                new Object[] { "BackgroundMode", BackgroundMode.Transparent},
               });
            ReflectInvoker.invoke("legendEntry3.TextFont", legendEntry3.TextFont, new Object[][]{
			    new Object[]{"Name", "Tahoma"},
			    new Object[]{"Size", 10},
			    new Object[]{"Underline", FontUnderlineType.Single},
			    new Object[]{"Color", Color.Black},
			    new Object[]{"IsBold", false},
			    new Object[]{"IsItalic", false},
			    new Object[]{"IsStrikeout", false},
			    new Object[]{"IsSubscript", false},
                new Object[] {"IsSuperscript", false}
			});

            LegendEntry legendEntry4 = legendEntries[3];
            ReflectInvoker.invoke("legendEntry4", legendEntry4, new Object[][]{
                new Object[] {"AutoScaleFont", false},
                new Object[] { "BackgroundMode", BackgroundMode.Automatic},
               });
            //CELLSNET-54094
            ReflectInvoker.invoke("legendEntry4.TextFont", legendEntry4.TextFont, new Object[][]{
                new Object[]{"Name", "Tahoma"},
                new Object[]{"Size", 10},
                new Object[]{"Underline", FontUnderlineType.None},
                new Object[]{"Color", Color.Black},
                new Object[]{"IsStrikeout", true},
                new Object[]{"IsSubscript", false},
                new Object[] {"IsSuperscript", false}
            });
            AssertHelper.AreEqual(true, legendEntry4.TextFont.IsBold && legendEntry4.TextFont.IsItalic, "legendEntry4.TextFont");

            LegendEntry legendEntry5 = legendEntries[4];
            ReflectInvoker.invoke("legendEntry5", legendEntry5, new Object[][]{
                new Object[] {"AutoScaleFont", false},
                new Object[] { "BackgroundMode", BackgroundMode.Opaque},
               });
            ReflectInvoker.invoke("legendEntry5.TextFont", legendEntry5.TextFont, new Object[][]{
			    new Object[]{"Name", "Tunga"},
			    new Object[]{"Size", 10},
			    new Object[]{"Underline", FontUnderlineType.Double},
			    new Object[]{"Color", Color.Black},
			    new Object[]{"IsBold", false},
			    new Object[]{"IsItalic", false},
			    new Object[]{"IsStrikeout", false},
			    new Object[]{"IsSubscript", true},
                new Object[] {"IsSuperscript", false}
			});                  
            //===============PlotArea=============================//
            AssertHelper.AreEqual(false, chart.PlotArea.Border.IsVisible, "chart.PlotArea.Border.IsVisible");
            AssertHelper.AreEqual(FormattingType.Automatic, chart.PlotArea.Area.Formatting, "chart.PlotArea.Area.Formatting");
            //==============CategoryAxis==========================//
            Axis categoryAxis = chart.CategoryAxis;
            //AssertHelper.assertEquals("categoryAxis.getAxisLine.isAuto", true, categoryAxis.getAxisLine().isAuto());
            ReflectInvoker.invoke("categoryAxis", categoryAxis, new Object[][]{
				new Object[] {"MajorTickMark", TickMarkType.Inside},
				new Object[] {"MinorTickMark", TickMarkType.None},				
				new Object[] {"TickLabelPosition", TickLabelPositionType.Low},
				new Object[] {"TickLabelSpacing", 1},
				new Object[] {"TickMarkSpacing", 1},
				new Object[] {"IsPlotOrderReversed", false},
				new Object[] {"AxisBetweenCategories", false},
                new Object[] {"IsVisible", true}
            });

            ReflectInvoker.invoke("categoryAxis.TickLabels", categoryAxis.TickLabels, new Object[][]{
			     new Object[]{"AutoScaleFont", false},
                 new Object[] { "BackgroundMode", BackgroundMode.Automatic},
                 new Object[] {"NumberFormatLinked", true},
                 new Object[] { "RotationAngle", 0},
                 new Object[] {"TextDirection", TextDirectionType.Context}
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

            Title categoryTitle = categoryAxis.Title;
            AssertHelper.AreEqual(false, categoryTitle.Border.IsVisible, "categoryTitle.Border.IsVisible");
            //AssertHelper.AreEqual(FormattingType.Automatic, categoryTitle.Area.Formatting, "categoryTitle.Area.Formatting");
            AssertHelper.AreEqual(FormattingType.None, categoryTitle.Area.Formatting, "categoryTitle.Area.Formatting");
            ReflectInvoker.invoke("categoryTitle", categoryTitle, new Object[][]{
				new Object[] {"Text", "Seconds"},
                new Object[] {"Shadow", false},
                new Object[] {"AutoScaleFont", false},
                new Object[] { "BackgroundMode", BackgroundMode.Automatic},
				new Object[]{"TextHorizontalAlignment", TextAlignmentType.Center},
				new Object[] {"TextVerticalAlignment", TextAlignmentType.Center},
				new Object[] {"TextDirection", TextDirectionType.Context},
				new Object[] { "RotationAngle", 0}
			});  
            ReflectInvoker.invoke("categoryTitle.TextFont", categoryTitle.TextFont, new Object[][]{
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
            //===============================
            Axis seriesAxis = chart.SeriesAxis;
            //AssertHelper.assertEquals("seriesAxis.getAxisLine.isAuto", true, seriesAxis.getAxisLine().isAuto());
            ReflectInvoker.invoke("seriesAxis", seriesAxis, new Object[][]{
				new Object[] {"MajorTickMark", TickMarkType.Inside},
				new Object[] {"MinorTickMark", TickMarkType.None},				
				new Object[] {"TickLabelPosition", TickLabelPositionType.Low},
				new Object[] {"TickLabelSpacing", 1},
				new Object[] {"TickMarkSpacing", 1},
				new Object[] {"IsPlotOrderReversed", false},
                new Object[] {"IsVisible", true}
				});
            ReflectInvoker.invoke("seriesAxis.TickLabels", seriesAxis.TickLabels, new Object[][]{
			    new Object[]{"AutoScaleFont", false},
                new Object[] { "BackgroundMode", BackgroundMode.Automatic},
                new Object[] {"NumberFormatLinked", true},
                new Object[] { "RotationAngle", 0},
                new Object[] {"TextDirection", TextDirectionType.Context}
              });
            ReflectInvoker.invoke("seriesAxis.TickLabels.Font", seriesAxis.TickLabels.Font, new Object[][]{
			new Object[]{"Name", "Tahoma"},
			new Object[]{"Size", 10},
			new Object[]{"Underline", FontUnderlineType.None},
			new Object[]{"Color", Color.Black},
			//new Object[]{"IsBold", true},
                new Object[]{"IsBold", false},
			new Object[]{"IsItalic", false},
			new Object[]{"IsStrikeout", false},
			new Object[]{"IsSubscript", false}
			});	
           

        }
```

### See Also

* class [Font](../../../aspose.cells/font/)
* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


