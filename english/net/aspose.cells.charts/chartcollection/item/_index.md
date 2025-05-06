---
title: ChartCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ChartCollection property. Gets the Chart element at the specified index
type: docs
url: /net/aspose.cells.charts/chartcollection/item/
---
## ChartCollection indexer (1 of 2)

Gets the [`Chart`](../../chart/) element at the specified index.

```csharp
public Chart this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp
// Called: Chart chart = sheet.Charts[0];
private void Property_Int32_(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[&quot;Sheet2&quot;];
            Chart chart = sheet.Charts[0];
            AssertHelper.AreEqual(ChartType.RadarWithDataMarkers, chart.Type, &quot;chart.Type&quot;);
        }
```

### See Also

* class [Chart](../../chart/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ChartCollection indexer (2 of 2)

Gets the chart by the name.

```csharp
public Chart this[string name] { get; }
```

| Parameter | Description |
| --- | --- |
| name | The chart name. |

### Return Value

The chart.

### Remarks

The default chart name is null. So you have to explicitly set the name of the chart.

### Examples

```csharp
// Called: Chart chart = workbook.Worksheets[&amp;quot;Ungleichheiten&amp;quot;].Charts[&amp;quot;Chart 1&amp;quot;];
[Test]
        public void Property_String_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsJava43372.ods&quot;);
            Chart chart = workbook.Worksheets[&quot;Ungleichheiten&quot;].Charts[&quot;Chart 1&quot;];
            Assert.AreEqual(4, chart.NSeries.Count);
            workbook.Save(Constants.destPath + &quot;CellsJava43372.xlsx&quot;);

        }
```

### See Also

* class [Chart](../../chart/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


