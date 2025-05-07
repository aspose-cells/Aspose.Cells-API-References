---
title: ChartTextFrame.IsResizeShapeToFitText
second_title: Aspose.Cells for .NET API Reference
description: ChartTextFrame property. Gets or sets whether a shape should be autofit to fully contain the text described within it. Autofitting is when text within a shape is scaled in order to contain all the text inside
type: docs
url: /net/aspose.cells.charts/charttextframe/isresizeshapetofittext/
---
## ChartTextFrame.IsResizeShapeToFitText property

Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting is when text within a shape is scaled in order to contain all the text inside.

```csharp
public bool IsResizeShapeToFitText { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(false, db00.IsResizeShapeToFitText);
[Test]
        public void Property_IsResizeShapeToFitText()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "Charts/ChartAPI/BarChart.xlsx");
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
            Assert.AreEqual("_(* #,##0_);_(* \\(#,##0\\);_(* \"-\"??_);_(@_)", db00.NumberFormat);
            Assert.AreEqual(true, db00.NumberFormatLinked);
            Assert.AreEqual(LabelPositionType.Center, db00.Position);
            Assert.AreEqual(TextDirectionType.LeftToRight, db00.ReadingOrder);
            Assert.AreEqual(0, db00.RotationAngle);
            Assert.AreEqual(DataLabelsSeparatorType.Auto, db00.SeparatorType);
            Assert.AreEqual("", db00.SeparatorValue);
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

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


