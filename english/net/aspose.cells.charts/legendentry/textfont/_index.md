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
// Called: ReflectInvoker.invoke(&amp;quot;legendEntry4.TextFont&amp;quot;, legendEntry4.TextFont, new Object[][]{
[Test]
        public void Property_TextFont()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Charts\\Contour.xls&quot;);
            Worksheet worksheet = workbook.Worksheets[0];
            Chart chart = worksheet.Charts[0];
            ReflectInvoker.invoke(&quot;chart&quot;, chart, new Object[][]{
			new Object[]{&quot;Type&quot;, ChartType.SurfaceContour},
            new Object[] {&quot;IsRectangularCornered&quot;, true},
            new Object[] { &quot;ShowLegend&quot;, true}});  
     
            ReflectInvoker.invoke(&quot;chart.ChartObject&quot;, chart.ChartObject, new Object[][]{
                new Object[] { &quot;IsPrintable&quot;, true},
			    new Object[]{&quot;IsLocked&quot;, true},
                new Object[] {&quot;Placement&quot;, PlacementType.Move}});
            //===============ChartArea==================//
            ChartArea chartArea = chart.ChartArea;
            //AssertHelper.assertEquals(&quot;chartArea.getBorder.isAuto&quot;, true, chartArea.getBorder().isAuto());
            AssertHelper.AreEqual(FormattingType.Automatic, chartArea.Area.Formatting, &quot;chartArea.getArea.isAuto&quot;);
            ReflectInvoker.invoke(&quot;chartArea&quot;, chartArea, new Object[][]{
				new Object[]{&quot;Shadow&quot;, false},
				new Object[]{&quot;AutoScaleFont&quot;, false},
				new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic},
			});               
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
            //===============Title=======================//
            Title title = chart.Title;
            AssertHelper.AreEqual(false, title.Border.IsVisible, &quot;title.Border.IsVisible&quot;);
            AssertHelper.AreEqual(FormattingType.None, title.Area.Formatting, &quot;title.Area.Formatting&quot;);
            ReflectInvoker.invoke(&quot;title&quot;, title, new Object[][]{                
				new Object[] {&quot;Text&quot;, &quot;Tensile strenth Measurements&quot;},
                new Object[] {&quot;Shadow&quot;, false},
                new Object[] {&quot;AutoScaleFont&quot;, false},
                new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic},
				new Object[]{&quot;TextHorizontalAlignment&quot;, TextAlignmentType.Center},
				new Object[] {&quot;TextVerticalAlignment&quot;, TextAlignmentType.Center},
				new Object[] {&quot;TextDirection&quot;, TextDirectionType.Context},
				new Object[] { &quot;RotationAngle&quot;, 0}
			});
            ReflectInvoker.invoke(&quot;title.TextFont&quot;, title.TextFont, new Object[][]{
			    new Object[]{&quot;Name&quot;, &quot;Arial&quot;},
			    new Object[]{&quot;Size&quot;, 12},
			    new Object[]{&quot;Underline&quot;, FontUnderlineType.None},
			    new Object[]{&quot;Color&quot;, Color.Black},
			    new Object[]{&quot;IsBold&quot;, true},
			    new Object[]{&quot;IsItalic&quot;, false},
			    new Object[]{&quot;IsStrikeout&quot;, false},
			    new Object[]{&quot;IsSubscript&quot;, false},
                new Object[] {&quot;IsSuperscript&quot;, false}
			});            
            //=====================Legend========================//
            Legend legend = chart.Legend;
            //AssertHelper.assertEquals(&quot;legend.getBorder.isAuto&quot;, true, legend.getBorder().isAuto());
            AssertHelper.AreEqual(FormattingType.Automatic, legend.Area.Formatting, &quot;legend.Area.Formatting&quot;);
            ReflectInvoker.invoke(&quot;legend&quot;, legend, new Object[][]{
                new Object[] {&quot;Shadow&quot;, false},
				new Object[]{&quot;Position&quot;, LegendPositionType.Right},
			});
            //=====================LegendEntry============//
            AssertHelper.AreEqual(5, legend.LegendEntries.Count, &quot;legend.LegendEntries.Count&quot;);
            LegendEntryCollection legendEntries = legend.LegendEntries;
            LegendEntry legendEntry1 = legendEntries[0];
            ReflectInvoker.invoke(&quot;legendEntry1&quot;, legendEntry1, new Object[][]{
                new Object[] {&quot;AutoScaleFont&quot;, true},
                new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic},
               });
            ReflectInvoker.invoke(&quot;legendEntry1.TextFont&quot;, legendEntry1.TextFont, new Object[][]{
			    new Object[]{&quot;Name&quot;, &quot;Tahoma&quot;},
			    new Object[]{&quot;Size&quot;, 10},
			    new Object[]{&quot;Underline&quot;, FontUnderlineType.None},
			    new Object[]{&quot;Color&quot;, Color.Red},
			    new Object[]{&quot;IsBold&quot;, false},
			    new Object[]{&quot;IsItalic&quot;, false},
			    new Object[]{&quot;IsStrikeout&quot;, false},
			    new Object[]{&quot;IsSubscript&quot;, false},
                new Object[] {&quot;IsSuperscript&quot;, false}
			});

            LegendEntry legendEntry2 = legendEntries[1];
            ReflectInvoker.invoke(&quot;legendEntry2&quot;, legendEntry2, new Object[][]{
                new Object[] {&quot;AutoScaleFont&quot;, false},
                new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic},
               });
            ReflectInvoker.invoke(&quot;legendEntry2.TextFont&quot;, legendEntry2.TextFont, new Object[][]{
			    new Object[]{&quot;Name&quot;, FontNameConstants.zh_HeiTi},
			    new Object[]{&quot;Size&quot;, 12},
			    new Object[]{&quot;Underline&quot;, FontUnderlineType.None},
			    new Object[]{&quot;Color&quot;, Color.Black},
			    new Object[]{&quot;IsBold&quot;, true},
			    new Object[]{&quot;IsItalic&quot;, false},
			    new Object[]{&quot;IsStrikeout&quot;, false},
			    new Object[]{&quot;IsSubscript&quot;, false},
                new Object[] {&quot;IsSuperscript&quot;, false}
			});

            LegendEntry legendEntry3 = legendEntries[2];
            ReflectInvoker.invoke(&quot;legendEntry3&quot;, legendEntry3, new Object[][]{
                new Object[] {&quot;AutoScaleFont&quot;, false},
                new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Transparent},
               });
            ReflectInvoker.invoke(&quot;legendEntry3.TextFont&quot;, legendEntry3.TextFont, new Object[][]{
			    new Object[]{&quot;Name&quot;, &quot;Tahoma&quot;},
			    new Object[]{&quot;Size&quot;, 10},
			    new Object[]{&quot;Underline&quot;, FontUnderlineType.Single},
			    new Object[]{&quot;Color&quot;, Color.Black},
			    new Object[]{&quot;IsBold&quot;, false},
			    new Object[]{&quot;IsItalic&quot;, false},
			    new Object[]{&quot;IsStrikeout&quot;, false},
			    new Object[]{&quot;IsSubscript&quot;, false},
                new Object[] {&quot;IsSuperscript&quot;, false}
			});

            LegendEntry legendEntry4 = legendEntries[3];
            ReflectInvoker.invoke(&quot;legendEntry4&quot;, legendEntry4, new Object[][]{
                new Object[] {&quot;AutoScaleFont&quot;, false},
                new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic},
               });
            //CELLSNET-54094
            ReflectInvoker.invoke(&quot;legendEntry4.TextFont&quot;, legendEntry4.TextFont, new Object[][]{
                new Object[]{&quot;Name&quot;, &quot;Tahoma&quot;},
                new Object[]{&quot;Size&quot;, 10},
                new Object[]{&quot;Underline&quot;, FontUnderlineType.None},
                new Object[]{&quot;Color&quot;, Color.Black},
                new Object[]{&quot;IsStrikeout&quot;, true},
                new Object[]{&quot;IsSubscript&quot;, false},
                new Object[] {&quot;IsSuperscript&quot;, false}
            });
            AssertHelper.AreEqual(true, legendEntry4.TextFont.IsBold &amp;&amp; legendEntry4.TextFont.IsItalic, &quot;legendEntry4.TextFont&quot;);

            LegendEntry legendEntry5 = legendEntries[4];
            ReflectInvoker.invoke(&quot;legendEntry5&quot;, legendEntry5, new Object[][]{
                new Object[] {&quot;AutoScaleFont&quot;, false},
                new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Opaque},
               });
            ReflectInvoker.invoke(&quot;legendEntry5.TextFont&quot;, legendEntry5.TextFont, new Object[][]{
			    new Object[]{&quot;Name&quot;, &quot;Tunga&quot;},
			    new Object[]{&quot;Size&quot;, 10},
			    new Object[]{&quot;Underline&quot;, FontUnderlineType.Double},
			    new Object[]{&quot;Color&quot;, Color.Black},
			    new Object[]{&quot;IsBold&quot;, false},
			    new Object[]{&quot;IsItalic&quot;, false},
			    new Object[]{&quot;IsStrikeout&quot;, false},
			    new Object[]{&quot;IsSubscript&quot;, true},
                new Object[] {&quot;IsSuperscript&quot;, false}
			});                  
            //===============PlotArea=============================//
            AssertHelper.AreEqual(false, chart.PlotArea.Border.IsVisible, &quot;chart.PlotArea.Border.IsVisible&quot;);
            AssertHelper.AreEqual(FormattingType.Automatic, chart.PlotArea.Area.Formatting, &quot;chart.PlotArea.Area.Formatting&quot;);
            //==============CategoryAxis==========================//
            Axis categoryAxis = chart.CategoryAxis;
            //AssertHelper.assertEquals(&quot;categoryAxis.getAxisLine.isAuto&quot;, true, categoryAxis.getAxisLine().isAuto());
            ReflectInvoker.invoke(&quot;categoryAxis&quot;, categoryAxis, new Object[][]{
				new Object[] {&quot;MajorTickMark&quot;, TickMarkType.Inside},
				new Object[] {&quot;MinorTickMark&quot;, TickMarkType.None},				
				new Object[] {&quot;TickLabelPosition&quot;, TickLabelPositionType.Low},
				new Object[] {&quot;TickLabelSpacing&quot;, 1},
				new Object[] {&quot;TickMarkSpacing&quot;, 1},
				new Object[] {&quot;IsPlotOrderReversed&quot;, false},
				new Object[] {&quot;AxisBetweenCategories&quot;, false},
                new Object[] {&quot;IsVisible&quot;, true}
            });

            ReflectInvoker.invoke(&quot;categoryAxis.TickLabels&quot;, categoryAxis.TickLabels, new Object[][]{
			     new Object[]{&quot;AutoScaleFont&quot;, false},
                 new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic},
                 new Object[] {&quot;NumberFormatLinked&quot;, true},
                 new Object[] { &quot;RotationAngle&quot;, 0},
                 new Object[] {&quot;TextDirection&quot;, TextDirectionType.Context}
             });
            ReflectInvoker.invoke(&quot;categoryAxis.TickLabels.Font&quot;, categoryAxis.TickLabels.Font, new Object[][]{
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

            Title categoryTitle = categoryAxis.Title;
            AssertHelper.AreEqual(false, categoryTitle.Border.IsVisible, &quot;categoryTitle.Border.IsVisible&quot;);
            //AssertHelper.AreEqual(FormattingType.Automatic, categoryTitle.Area.Formatting, &quot;categoryTitle.Area.Formatting&quot;);
            AssertHelper.AreEqual(FormattingType.None, categoryTitle.Area.Formatting, &quot;categoryTitle.Area.Formatting&quot;);
            ReflectInvoker.invoke(&quot;categoryTitle&quot;, categoryTitle, new Object[][]{
				new Object[] {&quot;Text&quot;, &quot;Seconds&quot;},
                new Object[] {&quot;Shadow&quot;, false},
                new Object[] {&quot;AutoScaleFont&quot;, false},
                new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic},
				new Object[]{&quot;TextHorizontalAlignment&quot;, TextAlignmentType.Center},
				new Object[] {&quot;TextVerticalAlignment&quot;, TextAlignmentType.Center},
				new Object[] {&quot;TextDirection&quot;, TextDirectionType.Context},
				new Object[] { &quot;RotationAngle&quot;, 0}
			});  
            ReflectInvoker.invoke(&quot;categoryTitle.TextFont&quot;, categoryTitle.TextFont, new Object[][]{
			    new Object[]{&quot;Name&quot;, &quot;Arial&quot;},
			    new Object[]{&quot;Size&quot;, 10},
			    new Object[]{&quot;Underline&quot;, FontUnderlineType.None},
			    new Object[]{&quot;Color&quot;, Color.Black},
			    new Object[]{&quot;IsBold&quot;, true},
			    new Object[]{&quot;IsItalic&quot;, false},
			    new Object[]{&quot;IsStrikeout&quot;, false},
			    new Object[]{&quot;IsSubscript&quot;, false},
                new Object[] {&quot;IsSuperscript&quot;, false}
			});   
            //===============================
            Axis seriesAxis = chart.SeriesAxis;
            //AssertHelper.assertEquals(&quot;seriesAxis.getAxisLine.isAuto&quot;, true, seriesAxis.getAxisLine().isAuto());
            ReflectInvoker.invoke(&quot;seriesAxis&quot;, seriesAxis, new Object[][]{
				new Object[] {&quot;MajorTickMark&quot;, TickMarkType.Inside},
				new Object[] {&quot;MinorTickMark&quot;, TickMarkType.None},				
				new Object[] {&quot;TickLabelPosition&quot;, TickLabelPositionType.Low},
				new Object[] {&quot;TickLabelSpacing&quot;, 1},
				new Object[] {&quot;TickMarkSpacing&quot;, 1},
				new Object[] {&quot;IsPlotOrderReversed&quot;, false},
                new Object[] {&quot;IsVisible&quot;, true}
				});
            ReflectInvoker.invoke(&quot;seriesAxis.TickLabels&quot;, seriesAxis.TickLabels, new Object[][]{
			    new Object[]{&quot;AutoScaleFont&quot;, false},
                new Object[] { &quot;BackgroundMode&quot;, BackgroundMode.Automatic},
                new Object[] {&quot;NumberFormatLinked&quot;, true},
                new Object[] { &quot;RotationAngle&quot;, 0},
                new Object[] {&quot;TextDirection&quot;, TextDirectionType.Context}
              });
            ReflectInvoker.invoke(&quot;seriesAxis.TickLabels.Font&quot;, seriesAxis.TickLabels.Font, new Object[][]{
			new Object[]{&quot;Name&quot;, &quot;Tahoma&quot;},
			new Object[]{&quot;Size&quot;, 10},
			new Object[]{&quot;Underline&quot;, FontUnderlineType.None},
			new Object[]{&quot;Color&quot;, Color.Black},
			//new Object[]{&quot;IsBold&quot;, true},
                new Object[]{&quot;IsBold&quot;, false},
			new Object[]{&quot;IsItalic&quot;, false},
			new Object[]{&quot;IsStrikeout&quot;, false},
			new Object[]{&quot;IsSubscript&quot;, false}
			});	
           

        }
```

### See Also

* class [Font](../../../aspose.cells/font/)
* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


