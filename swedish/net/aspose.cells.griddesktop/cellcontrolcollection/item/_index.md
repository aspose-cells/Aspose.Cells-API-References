---
title: "CellControlCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellControlCollection-egenskap. Hämtar cellkontrollen på angiven rad‑ och kolumn‑index"
type: docs
url: /sv/net/aspose.cells.griddesktop/cellcontrolcollection/item/
---
## CellControlCollection indexer (1 of 2)

Hämtar cellkontrollen på angiven rad‑ och kolumn‑index.

```csharp
public CellControl this[int row, int col] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| row | radindex. |
| kol | kolumnindex. |

### Anmärkningar

Om det inte finns ett CellControl-objekt på angivet rad‑kolumn‑index, kommer detta att kontrollera kolumnens CellControl‑objekt.

### Se även

* class [CellControl](../../cellcontrol/)
* class [CellControlCollection](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## CellControlCollection indexer (2 of 2)

Hämtar cellkontrollen med angivet cellnamn.

```csharp
public CellControl this[string cellName] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| cellName | cellnamn (i Excel-namnformat, som 'A1', 'F22') |

### Anmärkningar

Om det inte finns ett CellControl-objekt på angivet rad‑kolumn‑index, kommer detta att kontrollera kolumnens CellControl‑objekt.

### Se även

* class [CellControl](../../cellcontrol/)
* class [CellControlCollection](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


