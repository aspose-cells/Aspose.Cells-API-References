---
title: Add
second_title: Aspose.Cells för .NET API-referens
description: Lägg till en ny Slicer med pivottabell som datakälla
type: docs
weight: 20
url: /sv/net/aspose.cells.slicers/slicercollection/add/
---
## Add(PivotTable, string, string) {#add_5}

Lägg till en ny Slicer med pivottabell som datakälla

```csharp
public int Add(PivotTable pivot, string destCellName, string baseFieldName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivot | PivotTable | Pivottabellobjekt |
| destCellName | String | Cellen i det övre vänstra hörnet av Slicer-intervallet. |
| baseFieldName | String | Namnet på PivotField i PivotTable.BaseFields |

### Returvärde

Det nya add Slicer-indexet

### Exempel

```csharp

[C#]

slicers.Add(pivot, "E3", "fruit");
```

### Se även

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [SlicerCollection](../../slicercollection)
* namnutrymme [Aspose.Cells.Slicers](../../slicercollection)
* hopsättning [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, string) {#add_2}

Lägg till en ny Slicer med pivottabell som datakälla

```csharp
public int Add(PivotTable pivot, int row, int column, string baseFieldName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivot | PivotTable | Pivottabellobjekt |
| row | Int32 | Radindex för cellen i det övre vänstra hörnet av Slicer-området. |
| column | Int32 | Kolumnindex för cellen i det övre vänstra hörnet av Slicer-intervallet. |
| baseFieldName | String | Namnet på PivotField i PivotTable.BaseFields |

### Returvärde

Det nya add Slicer-indexet

### Exempel

```csharp

[C#]

slicers.Add(pivot, 20, 12, "fruit");
```

### Se även

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [SlicerCollection](../../slicercollection)
* namnutrymme [Aspose.Cells.Slicers](../../slicercollection)
* hopsättning [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, int) {#add_1}

Lägg till en ny Slicer med pivottabell som datakälla

```csharp
public int Add(PivotTable pivot, int row, int column, int baseFieldIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivot | PivotTable | Pivottabellobjekt |
| row | Int32 | Radindex för cellen i det övre vänstra hörnet av Slicer-området. |
| column | Int32 | Kolumnindex för cellen i det övre vänstra hörnet av Slicer-intervallet. |
| baseFieldIndex | Int32 | Indexet för PivotField i PivotTable.BaseFields |

### Returvärde

Det nya add Slicer-indexet

### Exempel

```csharp

[C#]

slicers.Add(pivot, 20, 8, 0);
```

### Se även

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [SlicerCollection](../../slicercollection)
* namnutrymme [Aspose.Cells.Slicers](../../slicercollection)
* hopsättning [Aspose.Cells](../../../)

---

## Add(PivotTable, string, int) {#add_4}

Lägg till en ny Slicer med pivottabell som datakälla

```csharp
public int Add(PivotTable pivot, string destCellName, int baseFieldIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivot | PivotTable | Pivottabellobjekt |
| destCellName | String | Cellen i det övre vänstra hörnet av Slicer-intervallet. |
| baseFieldIndex | Int32 | Indexet för PivotField i PivotTable.BaseFields |

### Returvärde

Det nya add Slicer-indexet

### Exempel

```csharp

[C#]

slicers.Add(pivot, "E20", 0);
```

### Se även

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [SlicerCollection](../../slicercollection)
* namnutrymme [Aspose.Cells.Slicers](../../slicercollection)
* hopsättning [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, PivotField) {#add}

Lägg till en ny Slicer med pivottabell som datakälla

```csharp
public int Add(PivotTable pivot, int row, int column, PivotField baseField)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivot | PivotTable | Pivottabellobjekt |
| row | Int32 | Radindex för cellen i det övre vänstra hörnet av Slicer-området. |
| column | Int32 | Kolumnindex för cellen i det övre vänstra hörnet av Slicer-intervallet. |
| baseField | PivotField | Pivotfältet i PivotTable.BaseFields |

### Returvärde

Det nya add Slicer-indexet

### Exempel

```csharp

[C#]

slicers.Add(pivot, 3, 12, pivot.BaseFields[0]);
```

### Se även

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [PivotField](../../../aspose.cells.pivot/pivotfield)
* class [SlicerCollection](../../slicercollection)
* namnutrymme [Aspose.Cells.Slicers](../../slicercollection)
* hopsättning [Aspose.Cells](../../../)

---

## Add(PivotTable, string, PivotField) {#add_3}

Lägg till en ny Slicer med pivottabell som datakälla

```csharp
public int Add(PivotTable pivot, string destCellName, PivotField baseField)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivot | PivotTable | Pivottabellobjekt |
| destCellName | String | Cellen i det övre vänstra hörnet av Slicer-intervallet. |
| baseField | PivotField | Pivotfältet i PivotTable.BaseFields |

### Returvärde

Det nya add Slicer-indexet

### Exempel

```csharp

[C#]

slicers.Add(pivot, "I3", pivot.BaseFields[0]);
```

### Se även

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [PivotField](../../../aspose.cells.pivot/pivotfield)
* class [SlicerCollection](../../slicercollection)
* namnutrymme [Aspose.Cells.Slicers](../../slicercollection)
* hopsättning [Aspose.Cells](../../../)

---

## Add(ListObject, int, string) {#add_8}

Lägg till en ny Slicer med ListObjet som datakälla

```csharp
public int Add(ListObject table, int index, string destCellName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| table | ListObject | ListObject-objekt |
| index | Int32 | Indexet för ListColumn i ListObject.ListColumns |
| destCellName | String | Cellen i det övre vänstra hörnet av Slicer-intervallet. |

### Returvärde

Det nya add Slicer-indexet

### Exempel

```csharp

[C#]

slicers.Add(table, 1, "E38");
```

### Se även

* class [ListObject](../../../aspose.cells.tables/listobject)
* class [SlicerCollection](../../slicercollection)
* namnutrymme [Aspose.Cells.Slicers](../../slicercollection)
* hopsättning [Aspose.Cells](../../../)

---

## Add(ListObject, ListColumn, string) {#add_7}

Lägg till en ny Slicer med ListObjet som datakälla

```csharp
public int Add(ListObject table, ListColumn listColumn, string destCellName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| table | ListObject | ListObject-objekt |
| listColumn | ListColumn | Listkolumnen i ListObject.ListColumns |
| destCellName | String | Cellen i det övre vänstra hörnet av Slicer-intervallet. |

### Returvärde

Det nya add Slicer-indexet

### Exempel

```csharp

[C#]

slicers.Add(table, table.ListColumns[1], "I38");
```

### Se även

* class [ListObject](../../../aspose.cells.tables/listobject)
* class [ListColumn](../../../aspose.cells.tables/listcolumn)
* class [SlicerCollection](../../slicercollection)
* namnutrymme [Aspose.Cells.Slicers](../../slicercollection)
* hopsättning [Aspose.Cells](../../../)

---

## Add(ListObject, ListColumn, int, int) {#add_6}

Lägg till en ny Slicer med ListObjet som datakälla

```csharp
public int Add(ListObject table, ListColumn listColumn, int row, int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| table | ListObject | ListObject-objekt |
| listColumn | ListColumn | Listkolumnen i ListObject.ListColumns |
| row | Int32 | Radindex för cellen i det övre vänstra hörnet av Slicer-området. |
| column | Int32 | Kolumnindex för cellen i det övre vänstra hörnet av Slicer-intervallet. |

### Returvärde

Det nya add Slicer-indexet

### Exempel

```csharp

[C#]

slicers.Add(table, table.ListColumns[1], 38, 12);
```

### Se även

* class [ListObject](../../../aspose.cells.tables/listobject)
* class [ListColumn](../../../aspose.cells.tables/listcolumn)
* class [SlicerCollection](../../slicercollection)
* namnutrymme [Aspose.Cells.Slicers](../../slicercollection)
* hopsättning [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
