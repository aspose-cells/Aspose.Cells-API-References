---
title: Add
second_title: Aspose.Cells für .NET-API-Referenz
description: Hinzufügen eines neuen Datenschnitts mit PivotTable als Datenquelle
type: docs
weight: 20
url: /de/net/aspose.cells.slicers/slicercollection/add/
---
## Add(PivotTable, string, string) {#add_5}

Hinzufügen eines neuen Datenschnitts mit PivotTable als Datenquelle

```csharp
public int Add(PivotTable pivot, string destCellName, string baseFieldName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivot | PivotTable | PivotTable-Objekt |
| destCellName | String | Die Zelle in der oberen linken Ecke des Slicer-Bereichs. |
| baseFieldName | String | Der Name von PivotField in PivotTable.BaseFields |

### Rückgabewert

Der neue Add-Slicer-Index

### Beispiele

```csharp

[C#]

slicers.Add(pivot, "E3", "fruit");
```

### Siehe auch

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [SlicerCollection](../../slicercollection)
* namensraum [Aspose.Cells.Slicers](../../slicercollection)
* Montage [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, string) {#add_2}

Hinzufügen eines neuen Datenschnitts mit PivotTable als Datenquelle

```csharp
public int Add(PivotTable pivot, int row, int column, string baseFieldName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivot | PivotTable | PivotTable-Objekt |
| row | Int32 | Zeilenindex der Zelle in der oberen linken Ecke des Slicer-Bereichs. |
| column | Int32 | Spaltenindex der Zelle in der oberen linken Ecke des Slicer-Bereichs. |
| baseFieldName | String | Der Name von PivotField in PivotTable.BaseFields |

### Rückgabewert

Der neue Add-Slicer-Index

### Beispiele

```csharp

[C#]

slicers.Add(pivot, 20, 12, "fruit");
```

### Siehe auch

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [SlicerCollection](../../slicercollection)
* namensraum [Aspose.Cells.Slicers](../../slicercollection)
* Montage [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, int) {#add_1}

Hinzufügen eines neuen Datenschnitts mit PivotTable als Datenquelle

```csharp
public int Add(PivotTable pivot, int row, int column, int baseFieldIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivot | PivotTable | PivotTable-Objekt |
| row | Int32 | Zeilenindex der Zelle in der oberen linken Ecke des Slicer-Bereichs. |
| column | Int32 | Spaltenindex der Zelle in der oberen linken Ecke des Slicer-Bereichs. |
| baseFieldIndex | Int32 | Der Index von PivotField in PivotTable.BaseFields |

### Rückgabewert

Der neue Add-Slicer-Index

### Beispiele

```csharp

[C#]

slicers.Add(pivot, 20, 8, 0);
```

### Siehe auch

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [SlicerCollection](../../slicercollection)
* namensraum [Aspose.Cells.Slicers](../../slicercollection)
* Montage [Aspose.Cells](../../../)

---

## Add(PivotTable, string, int) {#add_4}

Hinzufügen eines neuen Datenschnitts mit PivotTable als Datenquelle

```csharp
public int Add(PivotTable pivot, string destCellName, int baseFieldIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivot | PivotTable | PivotTable-Objekt |
| destCellName | String | Die Zelle in der oberen linken Ecke des Slicer-Bereichs. |
| baseFieldIndex | Int32 | Der Index von PivotField in PivotTable.BaseFields |

### Rückgabewert

Der neue Add-Slicer-Index

### Beispiele

```csharp

[C#]

slicers.Add(pivot, "E20", 0);
```

### Siehe auch

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [SlicerCollection](../../slicercollection)
* namensraum [Aspose.Cells.Slicers](../../slicercollection)
* Montage [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, PivotField) {#add}

Hinzufügen eines neuen Datenschnitts mit PivotTable als Datenquelle

```csharp
public int Add(PivotTable pivot, int row, int column, PivotField baseField)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivot | PivotTable | PivotTable-Objekt |
| row | Int32 | Zeilenindex der Zelle in der oberen linken Ecke des Slicer-Bereichs. |
| column | Int32 | Spaltenindex der Zelle in der oberen linken Ecke des Slicer-Bereichs. |
| baseField | PivotField | Das PivotField in PivotTable.BaseFields |

### Rückgabewert

Der neue Add-Slicer-Index

### Beispiele

```csharp

[C#]

slicers.Add(pivot, 3, 12, pivot.BaseFields[0]);
```

### Siehe auch

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [PivotField](../../../aspose.cells.pivot/pivotfield)
* class [SlicerCollection](../../slicercollection)
* namensraum [Aspose.Cells.Slicers](../../slicercollection)
* Montage [Aspose.Cells](../../../)

---

## Add(PivotTable, string, PivotField) {#add_3}

Hinzufügen eines neuen Datenschnitts mit PivotTable als Datenquelle

```csharp
public int Add(PivotTable pivot, string destCellName, PivotField baseField)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivot | PivotTable | PivotTable-Objekt |
| destCellName | String | Die Zelle in der oberen linken Ecke des Slicer-Bereichs. |
| baseField | PivotField | Das PivotField in PivotTable.BaseFields |

### Rückgabewert

Der neue Add-Slicer-Index

### Beispiele

```csharp

[C#]

slicers.Add(pivot, "I3", pivot.BaseFields[0]);
```

### Siehe auch

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [PivotField](../../../aspose.cells.pivot/pivotfield)
* class [SlicerCollection](../../slicercollection)
* namensraum [Aspose.Cells.Slicers](../../slicercollection)
* Montage [Aspose.Cells](../../../)

---

## Add(ListObject, int, string) {#add_8}

Neuen Slicer mit ListObjet als Datenquelle hinzufügen

```csharp
public int Add(ListObject table, int index, string destCellName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| table | ListObject | ListObject-Objekt |
| index | Int32 | Der Index von ListColumn in ListObject.ListColumns |
| destCellName | String | Die Zelle in der oberen linken Ecke des Slicer-Bereichs. |

### Rückgabewert

Der neue Add-Slicer-Index

### Beispiele

```csharp

[C#]

slicers.Add(table, 1, "E38");
```

### Siehe auch

* class [ListObject](../../../aspose.cells.tables/listobject)
* class [SlicerCollection](../../slicercollection)
* namensraum [Aspose.Cells.Slicers](../../slicercollection)
* Montage [Aspose.Cells](../../../)

---

## Add(ListObject, ListColumn, string) {#add_7}

Neuen Slicer mit ListObjet als Datenquelle hinzufügen

```csharp
public int Add(ListObject table, ListColumn listColumn, string destCellName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| table | ListObject | ListObject-Objekt |
| listColumn | ListColumn | Die ListColumn in ListObject.ListColumns |
| destCellName | String | Die Zelle in der oberen linken Ecke des Slicer-Bereichs. |

### Rückgabewert

Der neue Add-Slicer-Index

### Beispiele

```csharp

[C#]

slicers.Add(table, table.ListColumns[1], "I38");
```

### Siehe auch

* class [ListObject](../../../aspose.cells.tables/listobject)
* class [ListColumn](../../../aspose.cells.tables/listcolumn)
* class [SlicerCollection](../../slicercollection)
* namensraum [Aspose.Cells.Slicers](../../slicercollection)
* Montage [Aspose.Cells](../../../)

---

## Add(ListObject, ListColumn, int, int) {#add_6}

Neuen Slicer mit ListObjet als Datenquelle hinzufügen

```csharp
public int Add(ListObject table, ListColumn listColumn, int row, int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| table | ListObject | ListObject-Objekt |
| listColumn | ListColumn | Die ListColumn in ListObject.ListColumns |
| row | Int32 | Zeilenindex der Zelle in der oberen linken Ecke des Slicer-Bereichs. |
| column | Int32 | Spaltenindex der Zelle in der oberen linken Ecke des Slicer-Bereichs. |

### Rückgabewert

Der neue Add-Slicer-Index

### Beispiele

```csharp

[C#]

slicers.Add(table, table.ListColumns[1], 38, 12);
```

### Siehe auch

* class [ListObject](../../../aspose.cells.tables/listobject)
* class [ListColumn](../../../aspose.cells.tables/listcolumn)
* class [SlicerCollection](../../slicercollection)
* namensraum [Aspose.Cells.Slicers](../../slicercollection)
* Montage [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
