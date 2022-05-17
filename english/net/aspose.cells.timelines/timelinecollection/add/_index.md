---
title: Add
second_title: Aspose.Cells for .NET API Reference
description: 
type: docs
weight: 20
url: /net/aspose.cells.timelines/timelinecollection/add/
---
## TimelineCollection.Add method (1 of 6)

Add a new Timeline using PivotTable as data source

```csharp
public int Add(PivotTable pivot, int row, int column, string baseFieldName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| row | Int32 | Row index of the cell in the upper-left corner of the Timeline range. |
| column | Int32 | Column index of the cell in the upper-left corner of the Timeline range. |
| baseFieldName | String | The name of PivotField in PivotTable.BaseFields |

## Return Value

The new add Timeline index

### Examples

```csharp

[C#]
//Add a new Timeline using PivotTable as data source
sheet.Timelines.Add(pivot, 10, 5, "date");
```

### See Also

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [TimelineCollection](../../timelinecollection)
* namespace [Aspose.Cells.Timelines](../../timelinecollection)
* assembly [Aspose.Cells](../../../)

---

## TimelineCollection.Add method (2 of 6)

Add a new Timeline using PivotTable as data source

```csharp
public int Add(PivotTable pivot, string destCellName, string baseFieldName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| destCellName | String | The cell name in the upper-left corner of the Timeline range. |
| baseFieldName | String | The name of PivotField in PivotTable.BaseFields |

## Return Value

The new add Timeline index

### Examples

```csharp

[C#]
//Add a new Timeline using PivotTable as data source
sheet.Timelines.Add(pivot, "i15", "date");
```

### See Also

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [TimelineCollection](../../timelinecollection)
* namespace [Aspose.Cells.Timelines](../../timelinecollection)
* assembly [Aspose.Cells](../../../)

---

## TimelineCollection.Add method (3 of 6)

Add a new Timeline using PivotTable as data source

```csharp
public int Add(PivotTable pivot, int row, int column, int baseFieldIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| row | Int32 | Row index of the cell in the upper-left corner of the Timeline range. |
| column | Int32 | Column index of the cell in the upper-left corner of the Timeline range. |
| baseFieldIndex | Int32 | The index of PivotField in PivotTable.BaseFields |

## Return Value

The new add Timeline index

### Examples

```csharp

[C#]
//Add a new Timeline using PivotTable as data source
sheet.Timelines.Add(pivot, 15, 5, 1);
```

### See Also

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [TimelineCollection](../../timelinecollection)
* namespace [Aspose.Cells.Timelines](../../timelinecollection)
* assembly [Aspose.Cells](../../../)

---

## TimelineCollection.Add method (4 of 6)

Add a new Timeline using PivotTable as data source

```csharp
public int Add(PivotTable pivot, string destCellName, int baseFieldIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| destCellName | String | The cell name in the upper-left corner of the Timeline range. |
| baseFieldIndex | Int32 | The index of PivotField in PivotTable.BaseFields |

## Return Value

The new add Timeline index

### Examples

```csharp

[C#]
//Add a new Timeline using PivotTable as data source
sheet.Timelines.Add(pivot, "i5", 1);
```

### See Also

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [TimelineCollection](../../timelinecollection)
* namespace [Aspose.Cells.Timelines](../../timelinecollection)
* assembly [Aspose.Cells](../../../)

---

## TimelineCollection.Add method (5 of 6)

Add a new Timeline using PivotTable as data source

```csharp
public int Add(PivotTable pivot, int row, int column, PivotField baseField)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| row | Int32 | Row index of the cell in the upper-left corner of the Timeline range. |
| column | Int32 | Column index of the cell in the upper-left corner of the Timeline range. |
| baseField | PivotField | The PivotField in PivotTable.BaseFields |

## Return Value

The new add Timeline index

### Examples

```csharp

[C#]
//Add a new Timeline using PivotTable as data source
sheet.Timelines.Add(pivot, 20, 5, pivot.BaseFields[1]);
```

### See Also

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [PivotField](../../../aspose.cells.pivot/pivotfield)
* class [TimelineCollection](../../timelinecollection)
* namespace [Aspose.Cells.Timelines](../../timelinecollection)
* assembly [Aspose.Cells](../../../)

---

## TimelineCollection.Add method (6 of 6)

Add a new Timeline using PivotTable as data source

```csharp
public int Add(PivotTable pivot, string destCellName, PivotField baseField)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| destCellName | String | The cell name in the upper-left corner of the Timeline range. |
| baseField | PivotField | The PivotField in PivotTable.BaseFields |

## Return Value

The new add Timeline index

### Examples

```csharp

[C#]
//Add a new Timeline using PivotTable as data source
sheet.Timelines.Add(pivot, "i10", pivot.BaseFields[1]);
```

### See Also

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [PivotField](../../../aspose.cells.pivot/pivotfield)
* class [TimelineCollection](../../timelinecollection)
* namespace [Aspose.Cells.Timelines](../../timelinecollection)
* assembly [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
