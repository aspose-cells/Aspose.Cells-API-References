---
title: SparklineGroupCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: SparklineGroupCollection method. Adds an SparklineGroup with a Sparkline to the collection
type: docs
url: /net/aspose.cells.charts/sparklinegroupcollection/add/
---
## Add(SparklineType) {#add}

Adds an [`SparklineGroup`](../../sparklinegroup/) with a [`Sparkline`](../../sparkline/) to the collection.

```csharp
public int Add(SparklineType type)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | SparklineType | Specifies the type of the Sparkline group. |

### Return Value

[`SparklineGroup`](../../sparklinegroup/) object index.

### See Also

* enum [SparklineType](../../sparklinetype/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(SparklineType, string, bool, CellArea) {#add_1}

Adds an [`SparklineGroup`](../../sparklinegroup/) with [`Sparkline`](../../sparkline/) to the collection.

```csharp
public int Add(SparklineType type, string dataRange, bool isVertical, CellArea locationRange)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | SparklineType | Specifies the type of the Sparkline group. |
| dataRange | String | Specifies the data range of the sparkline group. |
| isVertical | Boolean | Specifies whether to plot the sparklines from the data range by row or by column. |
| locationRange | CellArea | Specifies where the sparklines to be placed. |

### Return Value

[`SparklineGroup`](../../sparklinegroup/) object index.

### Examples

```csharp
// Called: sheet.SparklineGroups.Add(SparklineType.Line, "A26385:C26385", false, CellArea.CreateCellArea("D26385", "D26385"));
[Test]
        public void Method_CellArea_()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.SparklineGroups.Add(SparklineType.Line, "A26385:C26385", false, CellArea.CreateCellArea("D26385", "D26385"));
            workbook.Save(Constants.destPath + "CELLSNET56012.xlsx");

        }
```

### See Also

* enum [SparklineType](../../sparklinetype/)
* struct [CellArea](../../../aspose.cells/cellarea/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


