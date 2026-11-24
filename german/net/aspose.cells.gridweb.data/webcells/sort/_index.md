---
title: "WebCells.Sort"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebCells-Methode. Sortiert die Daten von oben nach unten in einem Bereich eines WebWorksheet nach dem angegebenen Spaltenindex"
type: docs
url: /de/net/aspose.cells.gridweb.data/webcells/sort/
---
## Sort(int, int, int, int, int) {#sort}

Sortiert die Daten aufsteigend von oben nach unten in einem Bereich eines WebWorksheet nach angegebenem Spaltenindex.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int index)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | Int32 | Die Zeilennummer der ersten zu sortierenden Zelle. |
| startColumn | Int32 | Die Spaltennummer der ersten zu sortierenden Zelle. |
| Zeilen | Int32 | Anzahl der zu importierenden Zeilen. |
| Spalten | Int32 | Anzahl der zu importierenden Spalten. |
| Index | Int32 | Der Spaltenindex, der die Sortierspalte angibt. |

### Beispiele

```csharp

[C#]

GridWeb1.WebWorksheets[0].Cells.Sort(1,0,25,6,3);

[VB]

GridWeb1.WebWorksheets(0).Cells.Sort(1,0,25,6,3)

```

### Siehe auch

* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Sort(int, int, int, int, int, SortByOrder, SortOrientation, bool) {#sort_1}

Sortiert die Daten aufsteigend von oben nach unten in einem Bereich eines WebWorksheet nach angegebenem Spaltenindex.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int index, 
    SortByOrder sortOrder, SortOrientation sortOrientation, bool isCaseSensitive)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | Int32 | Die Zeilennummer der ersten zu sortierenden Zelle. |
| startColumn | Int32 | Die Spaltennummer der ersten zu sortierenden Zelle. |
| Zeilen | Int32 | Anzahl der zu importierenden Zeilen. |
| Spalten | Int32 | Anzahl der zu importierenden Spalten. |
| Index | Int32 | Der Spalten-(oder Zeilen-)Index, der die Sortierspalte (oder -zeile) angibt. Wenn die Sortierrichtung von oben nach unten ist, stellt der Index den Spaltenindex dar. Wenn die Sortierrichtung von links nach rechts ist, stellt der Index den Zeilenindex dar. |
| Reihenfolge | SortByOrder | Die Sortierreihenfolge: Aufsteigend oder Absteigend |
| Ausrichtung | SortOrientation | Die Sortierrichtung: von oben nach unten oder von links nach rechts. |
| isCaseSensitive | Boolean | Gibt an, ob die Sortierdaten bei Zeichenketten die Groß-/Kleinschreibung berücksichtigen. |

### Beispiele

```csharp

[C#]

GridWeb1.WebWorksheets[0].Cells.Sort(0,1,4,14,3,SortOrder.Ascending,SortOrientation.SortLeftToRight,true)

[VB]

GridWeb1.WebWorksheets(0).Cells.Sort(0,1,4,14,3,SortOrder.Ascending,SortOrientation.SortLeftToRight,True)

```

### Siehe auch

* enum [SortByOrder](../../sortbyorder/)
* enum [SortOrientation](../../sortorientation/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Sort(int, int, int, int, int[]) {#sort_2}

Sortiert die Daten aufsteigend von oben nach unten in einem Bereich eines WebWorksheet nach Feldern, die durch ein Array von Spaltenindizes angegeben sind.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int[] indexes)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | Int32 | Die Zeilennummer der ersten zu sortierenden Zelle. |
| startColumn | Int32 | Die Spaltennummer der ersten zu sortierenden Zelle. |
| Zeilen | Int32 | Anzahl der zu importierenden Zeilen. |
| Spalten | Int32 | Anzahl der zu importierenden Spalten. |
| Indizes | Int32[] | Das Array der Spaltenindizes, das angibt, nach welchen Daten sortiert wird. |

### Beispiele

```csharp

[C#]

int[] indexes = new int[3];
indexes[0] = 0;
indexes[1] = 2;
indexes[2] = 3;
GridWeb1.WebWorksheets[0].Cells.Sort(1,0,25,6,indexes);

[VB]

Dim indexes() As Integer =  New Integer(3) {} 
indexes(0) = 0
indexes(1) = 2
indexes(2) = 3
GridWeb1.WebWorksheets(0).Cells.Sort(1,0,25,6,indexes)

```

### Siehe auch

* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Sort(int, int, int, int, int[], SortByOrder[], SortOrientation, bool) {#sort_3}

Sortiert die Daten aufsteigend in einem Bereich eines WebWorksheet nach Feldern, die durch ein Index-Array angegeben sind.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int[] indexes, 
    SortByOrder[] orders, SortOrientation orientation, bool isCaseSensitive)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | Int32 | Die Zeilennummer der ersten zu sortierenden Zelle. |
| startColumn | Int32 | Die Spaltennummer der ersten zu sortierenden Zelle. |
| Zeilen | Int32 | Anzahl der zu importierenden Zeilen. |
| Spalten | Int32 | Anzahl der zu importierenden Spalten. |
| Indizes | Int32[] | Der Spalten-(oder Zeilen-)Index, der die Sortierspalte (oder -zeile) angibt. Wenn die Sortierrichtung von oben nach unten ist, stellt der Index den Spaltenindex dar. Wenn die Sortierrichtung von links nach rechts ist, stellt der Index den Zeilenindex dar. |
| Bestellungen | SortByOrder[] | Die Sortierreihenfolge: Aufsteigend oder Absteigend |
| Ausrichtung | SortOrientation | Die Sortierrichtung: von oben nach unten oder von links nach rechts. |
| isCaseSensitive | Boolean | Gibt an, ob die Sortierung die Groß-/Kleinschreibung berücksichtigt. |

### Hinweise

Wenn Sie diese Methode verwenden, um einen Datenblock zu sortieren, stellen Sie bitte sicher, dass die Länge des Parameters indexes der Länge des Parameters orders entspricht.

### Beispiele

```csharp

```

[C#] int[] indexes = new int[3]; indexes[0] = 0; indexes[1] = 1; indexes[2] = 3; SortOrder[] orders = new SortOrder[3]; orders[0] = SortOrder.Ascending; orders[1] = SortOrder.Descending; orders[2] = SortOrder.Descending; GridWeb1.WebWorksheets[0].Cells.Sort(0,1,4,14,indexes,orders,SortOrientation.SortLeftToRight,false); [VB] Dim indexes() As Integer = New Integer(3) {} indexes(0) = 0 indexes(1) = 1 indexes(2) = 3 Dim orders() As SortOrder = New SortOrder(3) {} orders(0) = SortOrder.Ascending orders(1) = SortOrder.Descending orders(2) = SortOrder.Descending GridWeb1.WebWorksheets(0).Cells.Sort(0,1,4,14,indexes,orders,SortOrientation.SortLeftToRight,False)

### Siehe auch

* enum [SortByOrder](../../sortbyorder/)
* enum [SortOrientation](../../sortorientation/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


