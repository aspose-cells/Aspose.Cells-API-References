---
title: "GridCells.Sort"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GridCells-Methode. Sortiert die Daten aufsteigend/absteigend von oben nach unten in einem Bereich eines Arbeitsblatts nach angegebenem Spaltenindex. Sortiert die Daten aufsteigend/absteigend von links nach rechts in einem Bereich eines Arbeitsblatts nach angegebenem Zeilenindex"
type: docs
url: /de/net/aspose.cells.griddesktop.data/gridcells/sort/
---
## Sort(int, int, int, int, int, bool, bool, bool) {#sort}

Sortiert die Daten aufsteigend/absteigend von oben nach unten in einem Bereich eines Arbeitsblatts nach angegebenem Spaltenindex. Sortiert die Daten aufsteigend/absteigend von links nach rechts in einem Bereich eines Arbeitsblatts nach angegebenem Zeilenindex.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int index, bool isAsending, 
    bool isCaseSensitive, bool islefttoright)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | Int32 | Die Zeilennummer der ersten zu sortierenden Zelle. |
| startColumn | Int32 | Die Spaltennummer der ersten zu sortierenden Zelle. |
| Zeilen | Int32 | Anzahl der zu importierenden Zeilen. |
| Spalten | Int32 | Anzahl der zu importierenden Spalten. |
| Index | Int32 | Der Spaltenindex, der die Sortierspalte angibt. Wenn die Orientierung von oben nach unten ist, steht er für den Spaltenindex, der die Sortierspalte angibt. Wenn die Orientierung von links nach rechts ist, steht er für den Zeilenindex, der die Sortierreihen angibt. |
| isAsending | Boolean | ob die Sortierreihenfolge aufsteigend ist . |
| isCaseSensitive | Boolean | ob die Sortierung groß-/kleinschreibungssensitiv ist . |
| islefttoright | Boolean | ob die Sortierausrichtung von links nach rechts ist |

### Beispiele

```csharp

 [C#]

 GridWeb1.WebWorksheets[0].Cells.Sort(1,0,25,6,3,true,true,false);

 [VB]

 GridWeb1.WebWorksheets(0).Cells.Sort(1,0,25,6,3,true,true,false)

```

### Siehe auch

* class [GridCells](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Sort(int, int, int, int, int[], SortOrder[], SortOrientation, bool) {#sort_1}

Sortiert die Daten des Bereichs.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int[] indexes, 
    SortOrder[] orders, SortOrientation orientation, bool isCaseSensitive)
```

| Parameter | Beschreibung |
| --- | --- |
| Zellen | Die Zellen enthalten den Datenbereich. |
| startRow | Die Startzeile des Bereichs. |
| startColumn | Die Startspalte des Bereichs. |
| Zeilen | die Gesamtzahl der Zeilen. |
| Spalten | Die Gesamtzahl der Spalten. |
| Indizes | Das sortierte Spaltenindex-Array |
| Bestellungen | Das sortierte Bestellungsarray |
| Ausrichtung | Die Sortierausrichtung: von links nach rechts oder von oben nach unten. |
| isCaseSensitive | Ob bei Zeichenfolgenvergleich die Groß-/Kleinschreibung berücksichtigt wird.. |

### Siehe auch

* enum [SortOrder](../../../aspose.cells.griddesktop/sortorder/)
* enum [SortOrientation](../../../aspose.cells.griddesktop/sortorientation/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


