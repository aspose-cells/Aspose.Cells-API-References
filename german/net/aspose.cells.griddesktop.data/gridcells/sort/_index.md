---
title: Sort
second_title: Aspose.Cells für .NET-API-Referenz
description: Sortiert die Daten aufsteigend/absteigend von oben nach unten in einem Bereich eines Arbeitsblatts nach dem angegebenen Spaltenindex. Sortiert die Daten aufsteigend/absteigend von links nach rechts in einem Bereich eines Arbeitsblatts nach dem angegebenen Zeilenindex.
type: docs
weight: 690
url: /de/net/aspose.cells.griddesktop.data/gridcells/sort/
---
## Sort(int, int, int, int, int, bool, bool, bool) {#sort}

Sortiert die Daten aufsteigend/absteigend von oben nach unten in einem Bereich eines Arbeitsblatts nach dem angegebenen Spaltenindex. Sortiert die Daten aufsteigend/absteigend von links nach rechts in einem Bereich eines Arbeitsblatts nach dem angegebenen Zeilenindex.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int index, bool isAsending, 
    bool isCaseSensitive, bool islefttoright)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | Int32 | Die Zeilennummer der ersten zu sortierenden Zelle. |
| startColumn | Int32 | Die Spaltennummer der ersten zu sortierenden Zelle. |
| rows | Int32 | Anzahl der zu importierenden Zeilen. |
| columns | Int32 | Anzahl der zu importierenden Spalten. |
| index | Int32 | Der Spaltenindex, der die Sortierspalte angibt. wenn die Ausrichtung von oben nach unten ist, steht er für den Spaltenindex, der die Sortierspalte angibt. wenn die Ausrichtung von links nach rechts ist, steht er für den Zeilenindex, der die Sortierung angibt die Zeile. |
| isAsending | Boolean | ob die Sortierreihenfolge aending ist . |
| isCaseSensitive | Boolean | ob bei der Sortierung zwischen Groß- und Kleinschreibung unterschieden wird. |
| islefttoright | Boolean | ob die Sortierrichtung von links nach rechts ist |

### Beispiele

```csharp

 [C#]

 GridWeb1.WebWorksheets[0].Cells.Sort(1,0,25,6,3,true,true,false);

 [VB]

 GridWeb1.WebWorksheets(0).Cells.Sort(1,0,25,6,3,true,true,false)

```

### Siehe auch

* class [GridCells](../../gridcells)
* namensraum [Aspose.Cells.GridDesktop.Data](../../gridcells)
* Montage [Aspose.Cells.GridDesktop](../../../)

---

## Sort(int, int, int, int, int[], SortOrder[], SortOrientation, bool) {#sort_1}

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int[] indexes, 
    SortOrder[] orders, SortOrientation orientation, bool isCaseSensitive)
```

### Siehe auch

* enum [SortOrder](../../../aspose.cells.griddesktop/sortorder)
* enum [SortOrientation](../../../aspose.cells.griddesktop/sortorientation)
* class [GridCells](../../gridcells)
* namensraum [Aspose.Cells.GridDesktop.Data](../../gridcells)
* Montage [Aspose.Cells.GridDesktop](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->