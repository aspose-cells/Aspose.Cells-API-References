---
title: SparklineCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: SparklineCollection property. Gets the Sparkline element at the specified index
type: docs
url: /net/aspose.cells.charts/sparklinecollection/item/
---
## SparklineCollection indexer

Gets the [`Sparkline`](../../sparkline/) element at the specified index.

```csharp
public Sparkline this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;Sheet1!D5:O5&amp;quot;, group.Sparklines[index].DataRange);
[Test]
        public void Property_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET58096.xlsx&quot;);

            // Access first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Access the first sparkline group
            SparklineGroup group = worksheet.SparklineGroups[0];

            // Add Data Ranges and Locations inside this sparkline group
            int index = group.Sparklines.Add(&quot;D5:O5&quot;, 4, 15);
            Assert.AreEqual(&quot;Sheet1!D5:O5&quot;, group.Sparklines[index].DataRange);
            //group.Sparklines.Add(&quot;D6:O6&quot;, 5, 15);
            //group.Sparklines.Add(&quot;D7:O7&quot;, 6, 15);
            //group.Sparklines.Add(&quot;D8:O8&quot;, 7, 15);

            // Save the workbook
            workbook.Save(Constants.destPath + &quot;CELLSNET58096.xlsb&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSNET58096.xlsb&quot;);
            group = worksheet.SparklineGroups[0];
            Assert.AreEqual(PlotEmptyCellsType.NotPlotted, group.PlotEmptyCellsType);
            workbook.Save(Constants.destPath + &quot;CELLSNET58096.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSNET58096.xlsx&quot;);
            group = worksheet.SparklineGroups[0];
            Assert.AreEqual(PlotEmptyCellsType.NotPlotted, group.PlotEmptyCellsType);
        }
```

### See Also

* class [Sparkline](../../sparkline/)
* class [SparklineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


