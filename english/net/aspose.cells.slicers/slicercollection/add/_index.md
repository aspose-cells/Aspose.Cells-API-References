---
title: SlicerCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: SlicerCollection method. Add a new Slicer using PivotTable as data source
type: docs
url: /net/aspose.cells.slicers/slicercollection/add/
---
## Add(PivotTable, string, string) {#add_5}

Add a new Slicer using PivotTable as data source

```csharp
public int Add(PivotTable pivot, string destCellName, string baseFieldName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| destCellName | String | The cell in the upper-left corner of the Slicer range. |
| baseFieldName | String | The name of PivotField in PivotTable.BaseFields |

### Return Value

The new add Slicer index

### Examples

```csharp

[C#]

slicers.Add(pivot, "E3", "fruit");
```

### See Also

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, string) {#add_2}

Add a new Slicer using PivotTable as data source

```csharp
public int Add(PivotTable pivot, int row, int column, string baseFieldName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| row | Int32 | Row index of the cell in the upper-left corner of the Slicer range. |
| column | Int32 | Column index of the cell in the upper-left corner of the Slicer range. |
| baseFieldName | String | The name of PivotField in PivotTable.BaseFields |

### Return Value

The new add Slicer index

### Examples

```csharp

[C#]

slicers.Add(pivot, 20, 12, "fruit");
```

### See Also

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, int) {#add_1}

Add a new Slicer using PivotTable as data source

```csharp
public int Add(PivotTable pivot, int row, int column, int baseFieldIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| row | Int32 | Row index of the cell in the upper-left corner of the Slicer range. |
| column | Int32 | Column index of the cell in the upper-left corner of the Slicer range. |
| baseFieldIndex | Int32 | The index of PivotField in PivotTable.BaseFields |

### Return Value

The new add Slicer index

### Examples

```csharp

[C#]

slicers.Add(pivot, 20, 8, 0);
```

### See Also

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, int) {#add_4}

Add a new Slicer using PivotTable as data source

```csharp
public int Add(PivotTable pivot, string destCellName, int baseFieldIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| destCellName | String | The cell in the upper-left corner of the Slicer range. |
| baseFieldIndex | Int32 | The index of PivotField in PivotTable.BaseFields |

### Return Value

The new add Slicer index

### Examples

```csharp

[C#]

slicers.Add(pivot, "E20", 0);
```

### See Also

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, PivotField) {#add}

Add a new Slicer using PivotTable as data source

```csharp
public int Add(PivotTable pivot, int row, int column, PivotField baseField)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| row | Int32 | Row index of the cell in the upper-left corner of the Slicer range. |
| column | Int32 | Column index of the cell in the upper-left corner of the Slicer range. |
| baseField | PivotField | The PivotField in PivotTable.BaseFields |

### Return Value

The new add Slicer index

### Examples

```csharp

[C#]

slicers.Add(pivot, 3, 12, pivot.BaseFields[0]);
```

### See Also

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, PivotField) {#add_3}

Add a new Slicer using PivotTable as data source

```csharp
public int Add(PivotTable pivot, string destCellName, PivotField baseField)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| destCellName | String | The cell in the upper-left corner of the Slicer range. |
| baseField | PivotField | The PivotField in PivotTable.BaseFields |

### Return Value

The new add Slicer index

### Examples

```csharp

[C#]

slicers.Add(pivot, "I3", pivot.BaseFields[0]);
```

### See Also

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(ListObject, int, string) {#add_8}

Add a new Slicer using ListObjet as data source

```csharp
public int Add(ListObject table, int index, string destCellName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| table | ListObject | ListObject object |
| index | Int32 | The index of ListColumn in ListObject.ListColumns |
| destCellName | String | The cell in the upper-left corner of the Slicer range. |

### Return Value

The new add Slicer index

### Examples

```csharp

[C#]

slicers.Add(table, 1, "E38");
```

### See Also

* class [ListObject](../../../aspose.cells.tables/listobject/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(ListObject, ListColumn, string) {#add_7}

Add a new Slicer using ListObjet as data source

```csharp
public int Add(ListObject table, ListColumn listColumn, string destCellName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| table | ListObject | ListObject object |
| listColumn | ListColumn | The ListColumn in ListObject.ListColumns |
| destCellName | String | The cell in the upper-left corner of the Slicer range. |

### Return Value

The new add Slicer index

### Examples

```csharp

[C#]

slicers.Add(table, table.ListColumns[1], "I38");
```

### See Also

* class [ListObject](../../../aspose.cells.tables/listobject/)
* class [ListColumn](../../../aspose.cells.tables/listcolumn/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(ListObject, ListColumn, int, int) {#add_6}

Add a new Slicer using ListObjet as data source

```csharp
public int Add(ListObject table, ListColumn listColumn, int row, int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| table | ListObject | ListObject object |
| listColumn | ListColumn | The ListColumn in ListObject.ListColumns |
| row | Int32 | Row index of the cell in the upper-left corner of the Slicer range. |
| column | Int32 | Column index of the cell in the upper-left corner of the Slicer range. |

### Return Value

The new add Slicer index

### Examples

```csharp

[C#]

slicers.Add(table, table.ListColumns[1], 38, 12);
```

### See Also

* class [ListObject](../../../aspose.cells.tables/listobject/)
* class [ListColumn](../../../aspose.cells.tables/listcolumn/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


