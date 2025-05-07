---
title: DataLabels.Number
second_title: Aspose.Cells for .NET API Reference
description: DataLabels property. Gets and sets the builtin number format
type: docs
url: /net/aspose.cells.charts/datalabels/number/
---
## DataLabels.Number property

Gets and sets the built-in number format.

```csharp
public int Number { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(0, db00.Number);
[Test]
        public void Property_Number()
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

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


