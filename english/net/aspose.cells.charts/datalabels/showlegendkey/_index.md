---
title: DataLabels.ShowLegendKey
second_title: Aspose.Cells for .NET API Reference
description: DataLabels property. Represents a specified charts data label legend key display behavior. True if the data label legend key is visible
type: docs
url: /net/aspose.cells.charts/datalabels/showlegendkey/
---
## DataLabels.ShowLegendKey property

Represents a specified chart's data label legend key display behavior. True if the data label legend key is visible.

```csharp
public bool ShowLegendKey { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(false, db00.ShowLegendKey);
[Test]
        public void Property_ShowLegendKey()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Charts/ChartAPI/BarChart.xlsx&quot;);
            Chart chart = workbook.Worksheets[0].Charts[0];
            SeriesCollection sc = chart.NSeries;

            DataLabels db00 = sc[0].DataLabels;
            Assert.AreEqual(false, db00.IsAutomaticRotation);
            Assert.AreEqual(true, db00.IsAutomaticSize);
            Assert.AreEqual(true, db00.IsAutoText);
            Assert.AreEqual(false, db00.IsDefaultPosBeSet);
            Assert.AreEqual(false, db00.IsDeleted);
            Assert.AreEqual(false, db00.IsInnerMode);
            Assert.AreEqual(false, db00.IsNeverOverlap);
            Assert.AreEqual(false, db00.IsResizeShapeToFitText);
            Assert.AreEqual(true, db00.IsTextWrapped);
            Assert.AreEqual(null, db00.LinkedSource);
            Assert.AreEqual(0, db00.Number);
            Assert.AreEqual(&quot;_(* #,##0_);_(* \\(#,##0\\);_(* \&quot;-\&quot;??_);_(@_)&quot;, db00.NumberFormat);
            Assert.AreEqual(true, db00.NumberFormatLinked);
            Assert.AreEqual(LabelPositionType.Center, db00.Position);
            Assert.AreEqual(TextDirectionType.LeftToRight, db00.ReadingOrder);
            Assert.AreEqual(0, db00.RotationAngle);
            Assert.AreEqual(DataLabelsSeparatorType.Auto, db00.SeparatorType);
            Assert.AreEqual(&quot;&quot;, db00.SeparatorValue);
            Assert.AreEqual(false, db00.Shadow);
            Assert.AreEqual(DataLabelShapeType.Rect, db00.ShapeType);
            Assert.AreEqual(false, db00.ShowBubbleSize);
            Assert.AreEqual(true, db00.ShowCategoryName);
            Assert.AreEqual(false, db00.ShowCellRange);
            Assert.AreEqual(false, db00.ShowLegendKey);
            Assert.AreEqual(false, db00.ShowPercentage);
            Assert.AreEqual(false, db00.ShowSeriesName);
            Assert.AreEqual(true, db00.ShowValue);
            Assert.AreEqual(null, db00.Text);
            Assert.AreEqual(TextAlignmentType.Center, db00.TextHorizontalAlignment);
            Assert.AreEqual(TextAlignmentType.Center, db00.TextVerticalAlignment);
        }
```

### See Also

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


