---
title: "GridCells.Sort"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridCells method. Sorterar data stigande/avtagande uppifrån och ner i ett område av ett Worksheet efter angivet kolumnindex. Sorterar data stigande/avtagande från vänster till höger i ett område av ett Worksheet efter angivet radindex."
type: docs
url: /sv/net/aspose.cells.griddesktop.data/gridcells/sort/
---
## Sort(int, int, int, int, int, bool, bool, bool) {#sort}

Sorterar data stigande/avtagande uppifrån och ner i ett område i ett kalkylblad efter angivet kolumnindex. Sorterar data stigande/avtagande vänster till höger i ett område i ett kalkylblad efter angivet radindex.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int index, bool isAsending, 
    bool isCaseSensitive, bool islefttoright)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRow | Int32 | Radnumret för den första cellen som ska sorteras. |
| startColumn | Int32 | Kolumnnumret för den första cellen som ska sorteras. |
| rader | Int32 | Antal rader att importera. |
| kolumner | Int32 | Antal kolumner att importera. |
| index | Int32 | Kolumnindex som specificerar sorteringskolumnen. Om orienteringen är uppifrån och ner står den för kolumnindex som specificerar sorteringskolumnen. Om orienteringen är från vänster till höger står den för radindex som specificerar sorteringsraden. |
| isAsending | Boolean | om sorteringsordningen är stigande. |
| isCaseSensitive | Boolean | om sorteringen är skiftlägeskänslig. |
| islefttoright | Boolean | om sorteringsorienteringen är från vänster till höger |

### Exempel

```csharp

 [C#]

 GridWeb1.WebWorksheets[0].Cells.Sort(1,0,25,6,3,true,true,false);

 [VB]

 GridWeb1.WebWorksheets(0).Cells.Sort(1,0,25,6,3,true,true,false)

```

### Se även

* class [GridCells](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Sort(int, int, int, int, int[], SortOrder[], SortOrientation, bool) {#sort_1}

Sorterar data i området.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int[] indexes, 
    SortOrder[] orders, SortOrientation orientation, bool isCaseSensitive)
```

| Parameter | Beskrivning |
| --- | --- |
| celler | Cellerna innehåller dataområdet. |
| startRow | Startraden för området. |
| startColumn | Startkolumnen för området. |
| rader | det totala antalet rader. |
| kolumner | Det totala antalet kolumner. |
| index | Den sorterade kolumnindexarrayen |
| ordningar | Den sorterade ordningsarrayen |
| orientering | sorteringsorienteringen: från vänster till höger eller från topp till botten. |
| isCaseSensitive | om skiftlägeskänslig vid jämförelse av sträng.. |

### Se även

* enum [SortOrder](../../../aspose.cells.griddesktop/sortorder/)
* enum [SortOrientation](../../../aspose.cells.griddesktop/sortorientation/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


