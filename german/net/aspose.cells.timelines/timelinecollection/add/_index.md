---
title: Add
second_title: Aspose.Cells für .NET-API-Referenz
description: Hinzufügen einer neuen Zeitachse mit PivotTable als Datenquelle
type: docs
weight: 20
url: /de/net/aspose.cells.timelines/timelinecollection/add/
---
## Add(PivotTable, int, int, string) {#add_2}

Hinzufügen einer neuen Zeitachse mit PivotTable als Datenquelle

```csharp
public int Add(PivotTable pivot, int row, int column, string baseFieldName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivot | PivotTable | PivotTable-Objekt |
| row | Int32 | Zeilenindex der Zelle in der oberen linken Ecke des Timeline-Bereichs. |
| column | Int32 | Spaltenindex der Zelle in der oberen linken Ecke des Timeline-Bereichs. |
| baseFieldName | String | Der Name von PivotField in PivotTable.BaseFields |

### Rückgabewert

Der neue Timeline-Index hinzufügen

### Beispiele

```csharp

[C#]
//Fügen Sie eine neue Zeitachse mit PivotTable als Datenquelle hinzu
sheet.Timelines.Add(pivot, 10, 5, "date");
```

### Siehe auch

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [TimelineCollection](../../timelinecollection)
* namensraum [Aspose.Cells.Timelines](../../timelinecollection)
* Montage [Aspose.Cells](../../../)

---

## Add(PivotTable, string, string) {#add_5}

Hinzufügen einer neuen Zeitachse mit PivotTable als Datenquelle

```csharp
public int Add(PivotTable pivot, string destCellName, string baseFieldName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivot | PivotTable | PivotTable-Objekt |
| destCellName | String | Der Zellenname in der oberen linken Ecke des Timeline-Bereichs. |
| baseFieldName | String | Der Name von PivotField in PivotTable.BaseFields |

### Rückgabewert

Der neue Timeline-Index hinzufügen

### Beispiele

```csharp

[C#]
//Fügen Sie eine neue Zeitachse mit PivotTable als Datenquelle hinzu
sheet.Timelines.Add(pivot, "i15", "date");
```

### Siehe auch

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [TimelineCollection](../../timelinecollection)
* namensraum [Aspose.Cells.Timelines](../../timelinecollection)
* Montage [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, int) {#add_1}

Hinzufügen einer neuen Zeitachse mit PivotTable als Datenquelle

```csharp
public int Add(PivotTable pivot, int row, int column, int baseFieldIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivot | PivotTable | PivotTable-Objekt |
| row | Int32 | Zeilenindex der Zelle in der oberen linken Ecke des Timeline-Bereichs. |
| column | Int32 | Spaltenindex der Zelle in der oberen linken Ecke des Timeline-Bereichs. |
| baseFieldIndex | Int32 | Der Index von PivotField in PivotTable.BaseFields |

### Rückgabewert

Der neue Timeline-Index hinzufügen

### Beispiele

```csharp

[C#]
//Fügen Sie eine neue Zeitachse mit PivotTable als Datenquelle hinzu
sheet.Timelines.Add(pivot, 15, 5, 1);
```

### Siehe auch

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [TimelineCollection](../../timelinecollection)
* namensraum [Aspose.Cells.Timelines](../../timelinecollection)
* Montage [Aspose.Cells](../../../)

---

## Add(PivotTable, string, int) {#add_4}

Hinzufügen einer neuen Zeitachse mit PivotTable als Datenquelle

```csharp
public int Add(PivotTable pivot, string destCellName, int baseFieldIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivot | PivotTable | PivotTable-Objekt |
| destCellName | String | Der Zellenname in der oberen linken Ecke des Timeline-Bereichs. |
| baseFieldIndex | Int32 | Der Index von PivotField in PivotTable.BaseFields |

### Rückgabewert

Der neue Timeline-Index hinzufügen

### Beispiele

```csharp

[C#]
//Fügen Sie eine neue Zeitachse mit PivotTable als Datenquelle hinzu
sheet.Timelines.Add(pivot, "i5", 1);
```

### Siehe auch

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [TimelineCollection](../../timelinecollection)
* namensraum [Aspose.Cells.Timelines](../../timelinecollection)
* Montage [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, PivotField) {#add}

Hinzufügen einer neuen Zeitachse mit PivotTable als Datenquelle

```csharp
public int Add(PivotTable pivot, int row, int column, PivotField baseField)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivot | PivotTable | PivotTable-Objekt |
| row | Int32 | Zeilenindex der Zelle in der oberen linken Ecke des Timeline-Bereichs. |
| column | Int32 | Spaltenindex der Zelle in der oberen linken Ecke des Timeline-Bereichs. |
| baseField | PivotField | Das PivotField in PivotTable.BaseFields |

### Rückgabewert

Der neue Timeline-Index hinzufügen

### Beispiele

```csharp

[C#]
//Fügen Sie eine neue Zeitachse mit PivotTable als Datenquelle hinzu
sheet.Timelines.Add(pivot, 20, 5, pivot.BaseFields[1]);
```

### Siehe auch

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [PivotField](../../../aspose.cells.pivot/pivotfield)
* class [TimelineCollection](../../timelinecollection)
* namensraum [Aspose.Cells.Timelines](../../timelinecollection)
* Montage [Aspose.Cells](../../../)

---

## Add(PivotTable, string, PivotField) {#add_3}

Hinzufügen einer neuen Zeitachse mit PivotTable als Datenquelle

```csharp
public int Add(PivotTable pivot, string destCellName, PivotField baseField)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pivot | PivotTable | PivotTable-Objekt |
| destCellName | String | Der Zellenname in der oberen linken Ecke des Timeline-Bereichs. |
| baseField | PivotField | Das PivotField in PivotTable.BaseFields |

### Rückgabewert

Der neue Timeline-Index hinzufügen

### Beispiele

```csharp

[C#]
//Fügen Sie eine neue Zeitachse mit PivotTable als Datenquelle hinzu
sheet.Timelines.Add(pivot, "i10", pivot.BaseFields[1]);
```

### Siehe auch

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [PivotField](../../../aspose.cells.pivot/pivotfield)
* class [TimelineCollection](../../timelinecollection)
* namensraum [Aspose.Cells.Timelines](../../timelinecollection)
* Montage [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
