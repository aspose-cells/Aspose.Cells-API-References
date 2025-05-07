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
// Called: Chart chart = sheet.Charts[sheet.Charts.Add(ChartType.Radar, 5, 2, 25, 11)];
public static Workbook Property_Int32_(Workbook workbook)
        {
            workbook = new Workbook(Constants.sourcePath + "Charts\\Radar\\Radar.xls");
            Worksheet sheet = workbook.Worksheets[0];
            Chart chart = sheet.Charts[sheet.Charts.Add(ChartType.Radar, 5, 2, 25, 11)];
            chart.NSeries.Add("=Sheet1!$A$2:$E$13", true);
            return workbook;
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
// Called: Chart chart = workbook.Worksheets[0].Charts["Chart 15"];
[Test]
        public void Property_String_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet50309.xlsx");
            Chart chart = workbook.Worksheets[0].Charts["Chart 15"];
            Assert.AreEqual(5, chart.Shapes.Count);
        }
```

### See Also

* class [Chart](../../chart/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


