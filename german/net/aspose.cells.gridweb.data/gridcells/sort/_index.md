---
title: "GridCells.Sort"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GridCells-Methode. Sortiert die Daten aufsteigend/absteigend von oben nach unten in einem Bereich eines Arbeitsblatts nach angegebenem Spaltenindex. Sortiert die Daten aufsteigend/absteigend von links nach rechts in einem Bereich eines Arbeitsblatts nach angegebenem Zeilenindex"
type: docs
url: /de/net/aspose.cells.gridweb.data/gridcells/sort/
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
 GridWeb GridWeb1 = new GridWeb();
 GridWeb1.WorkSheets[0].Cells.Sort(1,0,25,6,3,true,true,false);

 [VB]

 GridWeb1.WebWorksheets(0).Cells.Sort(1,0,25,6,3,true,true,false)

```

### Siehe auch

* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Sort(int, int, int, int, int[], SortByOrder[], SortOrientation, bool) {#sort_1}

Sortiert die Daten aufsteigend/absteigend von oben nach unten in einem Bereich eines Arbeitsblatts nach angegebenem Spaltenindex. Sortiert die Daten aufsteigend/absteigend von links nach rechts in einem Bereich eines Arbeitsblatts nach angegebenem Zeilenindex.

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
| Indizes | Int32[] | Das Spaltenindex-Array, das die Sortierspalte angibt. Wenn die Orientierung von oben nach unten ist, steht es für den Spaltenindex, der die Sortierspalte angibt. Wenn die Orientierung von links nach rechts ist, steht es für den Zeilenindex, der die Sortierreihenfolge angibt. |
| Bestellungen | SortByOrder[] | das das Sortierreihenfolge-Array . |
| Ausrichtung | SortOrientation | Sortierausrichtung |
| isCaseSensitive | Boolean | ob die Sortierung groß-/kleinschreibungssensitiv ist . |

### Beispiele

```csharp

 [C#]
 GridWeb GridWeb1=new GridWeb();
 int[] ids={0,1};
 SortByOrder[] sorder={SortByOrder.Ascending,SortByOrder.Descending};
 GridWeb1.WorkSheets[0].Cells.Sort(1,0,25,6,ids,sorder,SortOrientation.SortTopToBottom,false);

 [VB]

 GridWeb1.WorkSheets(0).Cells.Sort(1,0,25,6,ids,sorder,SortOrientation.SortTopToBottom,false)

```

### Siehe auch

* enum [SortByOrder](../../sortbyorder/)
* enum [SortOrientation](../../sortorientation/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


