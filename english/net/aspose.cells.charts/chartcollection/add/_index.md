---
title: ChartCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: ChartCollection method. Adds a chart to the collection
type: docs
url: /net/aspose.cells.charts/chartcollection/add/
---
## Add(ChartType, int, int, int, int) {#add}

Adds a chart to the collection.

```csharp
public int Add(ChartType type, int upperLeftRow, int upperLeftColumn, int lowerRightRow, 
    int lowerRightColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | ChartType | Chart type |
| upperLeftRow | Int32 | Upper left row index. |
| upperLeftColumn | Int32 | Upper left column index. |
| lowerRightRow | Int32 | Lower right row index |
| lowerRightColumn | Int32 | Lower right column index |

### Return Value

[`Chart`](../../chart/) object index.

### See Also

* enum [ChartType](../../charttype/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(ChartType, string, int, int, int, int) {#add_2}

Adds a chart to the collection.

```csharp
[Obsolete("Use ChartCollection.Add(ChartType, string, bool ,int , int, int, int ) instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(ChartType type, string dataRange, int topRow, int leftColumn, int rightRow, 
    int bottomColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | ChartType | Chart type |
| dataRange | String | Specifies the data range of the chart |
| topRow | Int32 | Upper left row index. |
| leftColumn | Int32 | Upper left column index. |
| rightRow | Int32 | Lower right row index |
| bottomColumn | Int32 | Lower right column index |

### Return Value

[`Chart`](../../chart/) object index.

### Remarks

NOTE: This member is now obsolete. Instead, please use `Add` property. This property will be removed 12 months later since May 2022. Aspose apologizes for any inconvenience you may have experienced.

### See Also

* enum [ChartType](../../charttype/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(byte[], string, bool, int, int, int, int) {#add_3}

Adds a chart with preset template.

```csharp
public int Add(byte[] data, string dataRange, bool isVertical, int topRow, int leftColumn, 
    int rightRow, int bottomColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| data | Byte[] | The data of chart template file(.crtx). |
| dataRange | String | Specifies the data range of the chart |
| isVertical | Boolean | Specifies whether to plot the series from a range of cell values by row or by column. |
| topRow | Int32 | Upper left row index. |
| leftColumn | Int32 | Upper left column index. |
| rightRow | Int32 | Lower right row index |
| bottomColumn | Int32 | Lower right column index |

### Return Value

[`Chart`](../../chart/) object index.

### See Also

* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(ChartType, string, bool, int, int, int, int) {#add_1}

Adds a chart to the collection.

```csharp
public int Add(ChartType type, string dataRange, bool isVertical, int topRow, int leftColumn, 
    int rightRow, int bottomColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | ChartType | Chart type |
| dataRange | String | Specifies the data range of the chart |
| isVertical | Boolean | Specifies whether to plot the series from a range of cell values by row or by column. |
| topRow | Int32 | Upper left row index. |
| leftColumn | Int32 | Upper left column index. |
| rightRow | Int32 | Lower right row index |
| bottomColumn | Int32 | Lower right column index |

### Return Value

[`Chart`](../../chart/) object index.

### See Also

* enum [ChartType](../../charttype/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


