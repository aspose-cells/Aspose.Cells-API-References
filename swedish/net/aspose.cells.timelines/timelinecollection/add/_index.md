---
title: Add
second_title: Aspose.Cells för .NET API-referens
description: Lägg till en ny tidslinje med pivottabell som datakälla
type: docs
weight: 20
url: /sv/net/aspose.cells.timelines/timelinecollection/add/
---
## Add(PivotTable, int, int, string) {#add_2}

Lägg till en ny tidslinje med pivottabell som datakälla

```csharp
public int Add(PivotTable pivot, int row, int column, string baseFieldName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivot | PivotTable | Pivottabellobjekt |
| row | Int32 | Radindex för cellen i det övre vänstra hörnet av tidslinjeintervallet. |
| column | Int32 | Kolumnindex för cellen i det övre vänstra hörnet av tidslinjeintervallet. |
| baseFieldName | String | Namnet på PivotField i PivotTable.BaseFields |

### Returvärde

Det nya lägg till tidslinjeindex

### Exempel

```csharp

[C#]
//Lägg till en ny tidslinje med pivottabell som datakälla
sheet.Timelines.Add(pivot, 10, 5, "date");
```

### Se även

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [TimelineCollection](../../timelinecollection)
* namnutrymme [Aspose.Cells.Timelines](../../timelinecollection)
* hopsättning [Aspose.Cells](../../../)

---

## Add(PivotTable, string, string) {#add_5}

Lägg till en ny tidslinje med pivottabell som datakälla

```csharp
public int Add(PivotTable pivot, string destCellName, string baseFieldName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivot | PivotTable | Pivottabellobjekt |
| destCellName | String | Cellnamnet i det övre vänstra hörnet av tidslinjeintervallet. |
| baseFieldName | String | Namnet på PivotField i PivotTable.BaseFields |

### Returvärde

Det nya lägg till tidslinjeindex

### Exempel

```csharp

[C#]
//Lägg till en ny tidslinje med pivottabell som datakälla
sheet.Timelines.Add(pivot, "i15", "date");
```

### Se även

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [TimelineCollection](../../timelinecollection)
* namnutrymme [Aspose.Cells.Timelines](../../timelinecollection)
* hopsättning [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, int) {#add_1}

Lägg till en ny tidslinje med pivottabell som datakälla

```csharp
public int Add(PivotTable pivot, int row, int column, int baseFieldIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivot | PivotTable | Pivottabellobjekt |
| row | Int32 | Radindex för cellen i det övre vänstra hörnet av tidslinjeintervallet. |
| column | Int32 | Kolumnindex för cellen i det övre vänstra hörnet av tidslinjeintervallet. |
| baseFieldIndex | Int32 | Indexet för PivotField i PivotTable.BaseFields |

### Returvärde

Det nya lägg till tidslinjeindex

### Exempel

```csharp

[C#]
//Lägg till en ny tidslinje med pivottabell som datakälla
sheet.Timelines.Add(pivot, 15, 5, 1);
```

### Se även

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [TimelineCollection](../../timelinecollection)
* namnutrymme [Aspose.Cells.Timelines](../../timelinecollection)
* hopsättning [Aspose.Cells](../../../)

---

## Add(PivotTable, string, int) {#add_4}

Lägg till en ny tidslinje med pivottabell som datakälla

```csharp
public int Add(PivotTable pivot, string destCellName, int baseFieldIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivot | PivotTable | Pivottabellobjekt |
| destCellName | String | Cellnamnet i det övre vänstra hörnet av tidslinjeintervallet. |
| baseFieldIndex | Int32 | Indexet för PivotField i PivotTable.BaseFields |

### Returvärde

Det nya lägg till tidslinjeindex

### Exempel

```csharp

[C#]
//Lägg till en ny tidslinje med pivottabell som datakälla
sheet.Timelines.Add(pivot, "i5", 1);
```

### Se även

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [TimelineCollection](../../timelinecollection)
* namnutrymme [Aspose.Cells.Timelines](../../timelinecollection)
* hopsättning [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, PivotField) {#add}

Lägg till en ny tidslinje med pivottabell som datakälla

```csharp
public int Add(PivotTable pivot, int row, int column, PivotField baseField)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivot | PivotTable | Pivottabellobjekt |
| row | Int32 | Radindex för cellen i det övre vänstra hörnet av tidslinjeintervallet. |
| column | Int32 | Kolumnindex för cellen i det övre vänstra hörnet av tidslinjeintervallet. |
| baseField | PivotField | Pivotfältet i PivotTable.BaseFields |

### Returvärde

Det nya lägg till tidslinjeindex

### Exempel

```csharp

[C#]
//Lägg till en ny tidslinje med pivottabell som datakälla
sheet.Timelines.Add(pivot, 20, 5, pivot.BaseFields[1]);
```

### Se även

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [PivotField](../../../aspose.cells.pivot/pivotfield)
* class [TimelineCollection](../../timelinecollection)
* namnutrymme [Aspose.Cells.Timelines](../../timelinecollection)
* hopsättning [Aspose.Cells](../../../)

---

## Add(PivotTable, string, PivotField) {#add_3}

Lägg till en ny tidslinje med pivottabell som datakälla

```csharp
public int Add(PivotTable pivot, string destCellName, PivotField baseField)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivot | PivotTable | Pivottabellobjekt |
| destCellName | String | Cellnamnet i det övre vänstra hörnet av tidslinjeintervallet. |
| baseField | PivotField | Pivotfältet i PivotTable.BaseFields |

### Returvärde

Det nya lägg till tidslinjeindex

### Exempel

```csharp

[C#]
//Lägg till en ny tidslinje med pivottabell som datakälla
sheet.Timelines.Add(pivot, "i10", pivot.BaseFields[1]);
```

### Se även

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [PivotField](../../../aspose.cells.pivot/pivotfield)
* class [TimelineCollection](../../timelinecollection)
* namnutrymme [Aspose.Cells.Timelines](../../timelinecollection)
* hopsättning [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
