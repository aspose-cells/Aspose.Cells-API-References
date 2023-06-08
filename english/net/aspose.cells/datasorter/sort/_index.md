---
title: DataSorter.Sort
second_title: Aspose.Cells for .NET API Reference
description: DataSorter method. Sorts the data of the area
type: docs
url: /net/aspose.cells/datasorter/sort/
---
## Sort(Cells, int, int, int, int) {#sort_2}

Sorts the data of the area.

```csharp
public int[] Sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cells | Cells | The cells contains the data area. |
| startRow | Int32 | The start row of the area. |
| startColumn | Int32 | The start column of the area. |
| endRow | Int32 | The end row of the area. |
| endColumn | Int32 | The end column of the area. |

### Return Value

the original indices(absolute position, for example, column A is 0, B is 1, ...) of the sorted rows/columns. If no rows/columns needs to be moved by this sorting operation, null will be returned.

### See Also

* class [Cells](../../cells/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Sort(Cells, CellArea) {#sort_1}

Sort the data of the area.

```csharp
public int[] Sort(Cells cells, CellArea area)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cells | Cells | The cells contains the data area. |
| area | CellArea | The area needed to sort |

### Return Value

the original indices(absolute position, for example, column A is 0, B is 1, ...) of the sorted rows/columns. If no rows/columns needs to be moved by this sorting operation, null will be returned.

### See Also

* class [Cells](../../cells/)
* struct [CellArea](../../cellarea/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Sort() {#sort}

Sort the data in the range.

```csharp
public int[] Sort()
```

### Return Value

the original indices(absolute position, for example, column A is 0, B is 1, ...) of the sorted rows/columns. If no rows/columns needs to be moved by this sorting operation, null will be returned.

### See Also

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


