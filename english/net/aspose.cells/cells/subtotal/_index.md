---
title: Cells.Subtotal
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Creates subtotals for the range
type: docs
url: /net/aspose.cells/cells/subtotal/
---
## Subtotal(CellArea, int, ConsolidationFunction, int[]) {#subtotal}

Creates subtotals for the range.

```csharp
public void Subtotal(CellArea ca, int groupBy, ConsolidationFunction function, int[] totalList)
```

| Parameter | Type | Description |
| --- | --- | --- |
| ca | CellArea | The range |
| groupBy | Int32 | The field to group by, as a zero-based integer offset |
| function | ConsolidationFunction | The subtotal function. |
| totalList | Int32[] | An array of zero-based field offsets, indicating the fields to which the subtotals are added. |

### See Also

* struct [CellArea](../../cellarea/)
* enum [ConsolidationFunction](../../consolidationfunction/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Subtotal(CellArea, int, ConsolidationFunction, int[], bool, bool, bool) {#subtotal_1}

Creates subtotals for the range.

```csharp
public void Subtotal(CellArea ca, int groupBy, ConsolidationFunction function, int[] totalList, 
    bool replace, bool pageBreaks, bool summaryBelowData)
```

| Parameter | Type | Description |
| --- | --- | --- |
| ca | CellArea | The range |
| groupBy | Int32 | The field to group by, as a zero-based integer offset |
| function | ConsolidationFunction | The subtotal function. |
| totalList | Int32[] | An array of zero-based field offsets, indicating the fields to which the subtotals are added. |
| replace | Boolean | Indicates whether replace the current subtotals |
| pageBreaks | Boolean | Indicates whether add page break between groups |
| summaryBelowData | Boolean | Indicates whether add summary below data. |

### See Also

* struct [CellArea](../../cellarea/)
* enum [ConsolidationFunction](../../consolidationfunction/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


