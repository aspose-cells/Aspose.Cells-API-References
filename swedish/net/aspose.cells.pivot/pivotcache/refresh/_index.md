---
title: "PivotCache.Refresh"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotCache method. Refreshes data from the data source and calculates data for the view of all pivottables which data source is this pivot cache"
type: docs
url: /sv/net/aspose.cells.pivot/pivotcache/refresh/
---
## Refresh(PivotTableRefreshOption) {#refresh_1}

Uppdaterar data från datakällan och beräknar data för vyn av alla pivottabeller vars datakälla är denna pivot cache.

```csharp
public PivotRefreshState Refresh(PivotTableRefreshOption option)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| alternativ | PivotTableRefreshOption | The options for refreshing data source of pivot table. |

### Anmärkningar

It's better that you can simply call [`RefreshAll`](../../../aspose.cells/workbook/refreshall/) to refresh all pivot tables and charts in the file.

### Se även

* enum [PivotRefreshState](../../pivotrefreshstate/)
* class [PivotTableRefreshOption](../../pivottablerefreshoption/)
* class [PivotCache](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Refresh() {#refresh}

Uppdaterar data från datakällan och beräknar data för vyn av alla pivottabeller vars datakälla är denna pivot cache.

```csharp
public PivotRefreshState Refresh()
```

### Anmärkningar

If both table1 and table2 use this cache, the two table will calculated. It's better that you can simply call [`RefreshAll`](../../../aspose.cells/workbook/refreshall/) to refresh all pivot tables and charts in the file.

### Se även

* enum [PivotRefreshState](../../pivotrefreshstate/)
* class [PivotCache](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


