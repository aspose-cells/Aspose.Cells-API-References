---
title: PlotArea.Height
second_title: Aspose.Cells for .NET API Reference
description: PlotArea property. Gets or sets the height of plotarea bounding box in units of 1/4000 of the chart area
type: docs
url: /net/aspose.cells.charts/plotarea/height/
---
## PlotArea.Height property

Gets or sets the height of plot-area bounding box in units of 1/4000 of the chart area.

```csharp
[Obsolete("Use PlotArea.HeightRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int Height { get; set; }
```

### Remarks

The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method.

The **X**, **Y**, **Width** and **Height** of **PlotArea** represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** and **InnerHeightRatioToChart** properties.

For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().

NOTE: This member is now obsolete. Please use PlotArea.HeightRatioToChart property, instead. Height = HeightRatioToChart * 4000. This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: Assert.AreEqual(3219, chart.PlotArea.Height); //skiasharp is 3181
        public void PlotArea_Property_Height()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
            Chart chart = workbook.Worksheets[0].Charts[0];
            chart.Calculate();

            Assert.AreEqual(1, chart.ChartArea.WidthRatioToChart);
            Assert.AreEqual(4000, chart.ChartArea.Height);

            Assert.AreEqual(2680, chart.PlotArea.Width);
#if !SKIA
            Assert.AreEqual(3219, chart.PlotArea.Height); //skiasharp is 3181
#endif
        }
```

### See Also

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


