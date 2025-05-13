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
// Called: Chart chart = workbook.Worksheets[0].Charts[0];
public void ChartCollection_Property_Item()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");

    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    Chart chart = workbook.Worksheets[0].Charts[0];
    Assert.AreEqual(TextAlignmentType.Left, chart.Title.TextHorizontalAlignment);
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
// Called: Assert.AreEqual(workbook.Worksheets[1].Charts["Gráfico 8A"].NSeries[0].HasLeaderLines, false);
public void ChartCollection_Property_Item()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Assert.AreEqual(workbook.Worksheets[1].Charts["Gráfico 8A"].NSeries[0].HasLeaderLines, false);
}
```

### See Also

* class [Chart](../../chart/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


