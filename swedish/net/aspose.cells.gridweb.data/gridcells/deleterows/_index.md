---
title: "GridCells.DeleteRows"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridCells-metod. Raderar flera rader"
type: docs
url: /sv/net/aspose.cells.gridweb.data/gridcells/deleterows/
---
## DeleteRows(int, int) {#deleterows}

Tar bort flera rader.

```csharp
public bool DeleteRows(int rowIndex, int totalRows)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | Int32 | Det första radindexet som ska raderas. |
| totalRows | Int32 | Antal rader som ska raderas. |

### Anmärkningar

Om det borttagna intervallet innehåller den övre delen (inte hela) av tabellen (ListObject), kan intervallet inte tas bort och inget görs. Det fungerar som i MS Excel.

### Se även

* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## DeleteRows(int, int, bool) {#deleterows_1}

Tar bort flera rader i kalkylbladet.

```csharp
public bool DeleteRows(int rowIndex, int totalRows, bool updateReference)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | Int32 | Radindex. |
| totalRows | Int32 | Antal rader som ska raderas. |
| updateReference | Boolean | Indikerar om referenser ska uppdateras i andra kalkylblad. |

### Se även

* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


