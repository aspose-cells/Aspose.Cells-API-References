---
title: "Worksheet.FreezePanes"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet‑metod. Fryser rutor på den angivna cellen i arbetsbladet"
type: docs
url: /sv/net/aspose.cells.griddesktop/worksheet/freezepanes/
---
## FreezePanes(string, int, int) {#freezepanes_1}

Fryser rutor vid den angivna cellen i kalkylbladet.

```csharp
public void FreezePanes(string cellName, int freezedRows, int freezedColumns)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellName | String | Cellnamn. |
| freezedRows | Int32 | Antal synliga rader i översta rutan, högst radindex. |
| freezedColumns | Int32 | Antal synliga kolumner i vänstra rutan, högst kolumnindex. |

### Anmärkningar

Radindex och kolumnindex kan inte alla vara noll. Antalet rader och antalet kolumner kan inte heller alla vara noll.

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## FreezePanes(int, int, int, int) {#freezepanes}

Fryser rutor vid den angivna cellen i kalkylbladet.

```csharp
public void FreezePanes(int row, int column, int freezedRows, int freezedColumns)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindex. |
| column | Int32 | Kolumnindex. |
| freezedRows | Int32 | Antal synliga rader i översta rutan, högst radindex. |
| freezedColumns | Int32 | Antal synliga kolumner i vänstra rutan, högst kolumnindex. |

### Anmärkningar

Radindex och kolumnindex kan inte alla vara noll. Antalet rader och antalet kolumner kan inte heller alla vara noll.

De två första parametrarna anger den frysta positionen och de två sista parametrarna anger det frysta området i det övre vänstra rutan.

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


