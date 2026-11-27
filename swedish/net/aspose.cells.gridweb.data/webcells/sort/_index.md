---
title: "WebCells.Sort"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebCells metod. Sorterar data stigande uppifrån och ner i ett område av ett WebWorksheet efter angivet kolumnindex"
type: docs
url: /sv/net/aspose.cells.gridweb.data/webcells/sort/
---
## Sort(int, int, int, int, int) {#sort}

Sorterar data stigande uppifrån och ner i ett område av ett WebWorksheet efter specificerat kolumnindex.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRow | Int32 | Radnumret för den första cellen som ska sorteras. |
| startColumn | Int32 | Kolumnnumret för den första cellen som ska sorteras. |
| rader | Int32 | Antal rader att importera. |
| kolumner | Int32 | Antal kolumner att importera. |
| index | Int32 | Kolumnindexet som specificerar sorteringskolumnen. |

### Exempel

```csharp

[C#]

GridWeb1.WebWorksheets[0].Cells.Sort(1,0,25,6,3);

[VB]

GridWeb1.WebWorksheets(0).Cells.Sort(1,0,25,6,3)

```

### Se även

* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Sort(int, int, int, int, int, SortByOrder, SortOrientation, bool) {#sort_1}

Sorterar data stigande uppifrån och ner i ett område av ett WebWorksheet efter specificerat kolumnindex.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int index, 
    SortByOrder sortOrder, SortOrientation sortOrientation, bool isCaseSensitive)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRow | Int32 | Radnumret för den första cellen som ska sorteras. |
| startColumn | Int32 | Kolumnnumret för den första cellen som ska sorteras. |
| rader | Int32 | Antal rader att importera. |
| kolumner | Int32 | Antal kolumner att importera. |
| index | Int32 | Kolumn‑(eller rad‑)indexet som specificerar sorteringskolumnen (eller raden). Om sorteringsorienteringen är uppifrån och ner representerar indexet ett kolumnindex. Om sorteringsorienteringen är vänster till höger representerar indexet ett radindex. |
| ordning | SortByOrder | Sorteringsordning: Stigande eller Fallande |
| orientering | SortOrientation | Sorteringsorientering: uppifrån och ner eller vänster till höger. |
| isCaseSensitive | Boolean | Anger om sorteringsdata är skiftlägeskänslig när data är en sträng. |

### Exempel

```csharp

[C#]

GridWeb1.WebWorksheets[0].Cells.Sort(0,1,4,14,3,SortOrder.Ascending,SortOrientation.SortLeftToRight,true)

[VB]

GridWeb1.WebWorksheets(0).Cells.Sort(0,1,4,14,3,SortOrder.Ascending,SortOrientation.SortLeftToRight,True)

```

### Se även

* enum [SortByOrder](../../sortbyorder/)
* enum [SortOrientation](../../sortorientation/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Sort(int, int, int, int, int[]) {#sort_2}

Sorterar data stigande uppifrån och ner i ett område av ett WebWorksheet efter några fält som specificeras av en array med kolumnindex.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int[] indexes)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRow | Int32 | Radnumret för den första cellen som ska sorteras. |
| startColumn | Int32 | Kolumnnumret för den första cellen som ska sorteras. |
| rader | Int32 | Antal rader att importera. |
| kolumner | Int32 | Antal kolumner att importera. |
| index | Int32[] | Arrayen med kolumnindex som specificerar vilka data som sorteras. |

### Exempel

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

### Se även

* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Sort(int, int, int, int, int[], SortByOrder[], SortOrientation, bool) {#sort_3}

Sorterar data stigande i ett område av ett WebWorksheet efter några fält som specificeras av en indexarray.

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
| index | Int32[] | Kolumn‑(eller rad‑)indexet som specificerar sorteringskolumnen (eller raden). Om sorteringsorienteringen är uppifrån och ner representerar indexet ett kolumnindex. Om sorteringsorienteringen är vänster till höger representerar indexet ett radindex. |
| ordningar | SortByOrder[] | Sorteringsordning: Stigande eller Fallande |
| orientering | SortOrientation | Sorteringsorientering: uppifrån och ner eller vänster till höger. |
| isCaseSensitive | Boolean | Anger om sorteringen är skiftlägeskänslig. |

### Anmärkningar

Om du använder den här metoden för att sortera ett block med data, se till att längden på parametern indexer är lika med längden på parametern ordningar.

### Exempel

```csharp

```

[C#] int[] indexes = new int[3]; indexes[0] = 0; indexes[1] = 1; indexes[2] = 3; SortOrder[] orders = new SortOrder[3]; orders[0] = SortOrder.Ascending; orders[1] = SortOrder.Descending; orders[2] = SortOrder.Descending; GridWeb1.WebWorksheets[0].Cells.Sort(0,1,4,14,indexes,orders,SortOrientation.SortLeftToRight,false); [VB] Dim indexes() As Integer = New Integer(3) {} indexes(0) = 0 indexes(1) = 1 indexes(2) = 3 Dim orders() As SortOrder = New SortOrder(3) {} orders(0) = SortOrder.Ascending orders(1) = SortOrder.Descending orders(2) = SortOrder.Descending GridWeb1.WebWorksheets(0).Cells.Sort(0,1,4,14,indexes,orders,SortOrientation.SortLeftToRight,False)

### Se även

* enum [SortByOrder](../../sortbyorder/)
* enum [SortOrientation](../../sortorientation/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


