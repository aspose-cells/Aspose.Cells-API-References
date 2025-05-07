---
title: Marker.MarkerStyle
second_title: Aspose.Cells for .NET API Reference
description: Marker property. Represents the marker style. Applies to line chart scatter chart or radar chart
type: docs
url: /net/aspose.cells.charts/marker/markerstyle/
---
## Marker.MarkerStyle property

Represents the marker style. Applies to line chart, scatter chart, or radar chart.

```csharp
public ChartMarkerType MarkerStyle { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(ChartMarkerType.None, chart.NSeries[0].Points[7].Marker.MarkerStyle);
[Test]
        public void Property_MarkerStyle()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet55543.xlsx");
            Workbook wb = new Workbook();
            foreach (Worksheet sheet in workbook.Worksheets)
            {
                Worksheet ws = wb.Worksheets.Add(sheet.Name);

            }

            foreach (Worksheet sheet in workbook.Worksheets)
            {
                Worksheet ws = wb.Worksheets[sheet.Name];
                ws.Copy(sheet);
            }
            wb.Save(Constants.destPath + "CellsNet55543.xlsx");
            workbook = new Workbook(Constants.destPath + "CellsNet55543.xlsx");
            Chart chart = workbook.Worksheets[2].Charts[0];
            Assert.AreEqual(FillType.None, chart.ChartArea.Area.FillFormat.FillType);
            //  Assert.IsTrue(Util.CompareColor(Color.Blue, chart.NSeries[0].Points[7].Marker.ForegroundColor));
            Assert.AreEqual(ChartMarkerType.Circle, chart.NSeries[0].Points[3].Marker.MarkerStyle);
            Assert.AreEqual(ChartMarkerType.None, chart.NSeries[0].Points[7].Marker.MarkerStyle);
        }
```

### See Also

* enum [ChartMarkerType](../../chartmarkertype/)
* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


