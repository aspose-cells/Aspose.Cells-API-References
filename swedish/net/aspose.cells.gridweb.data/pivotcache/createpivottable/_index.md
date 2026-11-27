---
title: "PivotCache.CreatePivotTable"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotCache-metod. Skapar en PivotTable‑rapport på ett nytt ark"
type: docs
url: /sv/net/aspose.cells.gridweb.data/pivotcache/createpivottable/
---
## CreatePivotTable() {#createpivottable}

Skapar en PivotTable-rapport till ett nytt blad.

```csharp
public PivotTable CreatePivotTable()
```

### Returvärde

PivotTable‑objektet

### Anmärkningar

Genom att anropa den här metoden skapas ett PivotTable‑objekt och ett nytt arbetsblad. Därefter läggs PivotTable‑objektet till på den sista platsen i GridWeb.Worksheets.PivotTables. Om du anropar PivotTable.DataBind()-metoden kommer PivotTable‑rapporten att ritas på det skapade arbetsbladet.

### Se även

* class [PivotTable](../../pivottable/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## CreatePivotTable(string) {#createpivottable_3}

Skapar en PivotTable-rapport till ett nytt blad. Namnet på pivotTable-objektet

```csharp
public PivotTable CreatePivotTable(string tableName)
```

### Returvärde

PivotTable‑objektet

### Anmärkningar

Genom att anropa den här metoden skapas ett PivotTable‑objekt och ett nytt arbetsblad. Därefter läggs PivotTable‑objektet till på den sista platsen i GridWeb.Worksheets.PivotTables. Om du anropar PivotTable.DataBind()-metoden kommer PivotTable‑rapporten att ritas på det skapade arbetsbladet.

### Se även

* class [PivotTable](../../pivottable/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## CreatePivotTable(WebWorksheet, WebCell) {#createpivottable_1}

Skapar en PivotTable-rapport till targetSheet.

```csharp
public PivotTable CreatePivotTable(WebWorksheet targetSheet, WebCell targetCell)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| targetSheet | WebWorksheet | Arket som pivotTable‑rapporten kommer att ritas på |
| targetCell | WebCell | Startcellen som pivotTable‑rapporten kommer att ritas på |

### Returvärde

PivotTable‑objektet

### Anmärkningar

Genom att anropa den här metoden skapas ett PivotTable‑objekt. Därefter läggs PivotTable‑objektet till på den sista platsen i GridWeb.Worksheets.PivotTables. Om du anropar PivotTable.DataBind()-metoden kommer PivotTable‑rapporten att ritas på targetSheet med start i targetCell.

### Se även

* class [PivotTable](../../pivottable/)
* class [WebWorksheet](../../webworksheet/)
* class [WebCell](../../webcell/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## CreatePivotTable(WebWorksheet, WebCell, string) {#createpivottable_2}

Skapar en PivotTable-rapport till targetSheet.

```csharp
public PivotTable CreatePivotTable(WebWorksheet targetSheet, WebCell targetCell, string tableName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| targetSheet | WebWorksheet | Arket som pivotTable‑rapporten kommer att ritas på |
| targetCell | WebCell | Startcellen som pivotTable‑rapporten kommer att ritas på |
| tableName | String | Namnet på pivotTable-objektet |

### Returvärde

PivotTable‑objektet

### Anmärkningar

Att anropa den här metoden kommer att skapa ett PivotTable-objekt med namnet tableName och sedan lägga till PivotTable-objektet på den sista platsen i GridWeb.Worksheets.PivotTables. Om du anropar metoden PivotTable.DataBind() kommer PivotTable-rapporten att ritas på targetSheet med början i targetCell.

### Se även

* class [PivotTable](../../pivottable/)
* class [WebWorksheet](../../webworksheet/)
* class [WebCell](../../webcell/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


