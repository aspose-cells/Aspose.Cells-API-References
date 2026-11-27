---
title: "GridCells.Sort"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridCells method. Sorterar data stigande/avtagande uppifrån och ner i ett område av ett Worksheet efter angivet kolumnindex. Sorterar data stigande/avtagande från vänster till höger i ett område av ett Worksheet efter angivet radindex."
type: docs
url: /sv/net/aspose.cells.gridweb.data/gridcells/sort/
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
 GridWeb GridWeb1 = new GridWeb();
 GridWeb1.WorkSheets[0].Cells.Sort(1,0,25,6,3,true,true,false);

 [VB]

 GridWeb1.WebWorksheets(0).Cells.Sort(1,0,25,6,3,true,true,false)

```

### Se även

* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Sort(int, int, int, int, int[], SortByOrder[], SortOrientation, bool) {#sort_1}

Sorterar data stigande/avtagande uppifrån och ner i ett område i ett kalkylblad efter angivet kolumnindex. Sorterar data stigande/avtagande vänster till höger i ett område i ett kalkylblad efter angivet radindex.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int[] indexes, 
    SortByOrder[] orders, SortOrientation orientation, bool isCaseSensitive)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRow | Int32 | Radnumret för den första cellen som ska sorteras. |
| startColumn | Int32 | Kolumnnumret för den första cellen som ska sorteras. |
| rader | Int32 | Antal rader att importera. |
| kolumner | Int32 | Antal kolumner att importera. |
| index | Int32[] | Kolumnindexarrayen som specificerar sorteringskolumnen. Om Orientation är top to bottom, representerar den kolumnindexet som specificerar sorteringskolumnen. Om Orientation är from left to right, representerar den radindexet som specificerar sorteringsraden. |
| ordningar | SortByOrder[] | sorteringsordningsarrayen. |
| orientering | SortOrientation | sorteringsorientering |
| isCaseSensitive | Boolean | om sorteringen är skiftlägeskänslig. |

### Exempel

```csharp

 [C#]
 GridWeb GridWeb1=new GridWeb();
 int[] ids={0,1};
 SortByOrder[] sorder={SortByOrder.Ascending,SortByOrder.Descending};
 GridWeb1.WorkSheets[0].Cells.Sort(1,0,25,6,ids,sorder,SortOrientation.SortTopToBottom,false);

 [VB]

 GridWeb1.WorkSheets(0).Cells.Sort(1,0,25,6,ids,sorder,SortOrientation.SortTopToBottom,false)

```

### Se även

* enum [SortByOrder](../../sortbyorder/)
* enum [SortOrientation](../../sortorientation/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


