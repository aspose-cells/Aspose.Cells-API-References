---
title: "PivotCache.Refresh"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotCache-Methode. Aktualisiert Daten aus der Datenquelle und berechnet Daten für die Ansicht aller PivotTables, deren Datenquelle dieser Pivot-Cache ist."
type: docs
url: /de/net/aspose.cells.pivot/pivotcache/refresh/
---
## Refresh(PivotTableRefreshOption) {#refresh_1}

Aktualisiert Daten aus der Datenquelle und berechnet Daten für die Ansicht aller Pivot-Tabellen, deren Datenquelle dieser Pivot-Cache ist.

```csharp
public PivotRefreshState Refresh(PivotTableRefreshOption option)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Option | PivotTableRefreshOption | Die Optionen zum Aktualisieren der Datenquelle der PivotTable. |

### Hinweise

Es ist besser, wenn Sie einfach [`RefreshAll`](../../../aspose.cells/workbook/refreshall/) aufrufen, um alle PivotTables und Diagramme in der Datei zu aktualisieren.

### Siehe auch

* enum [PivotRefreshState](../../pivotrefreshstate/)
* class [PivotTableRefreshOption](../../pivottablerefreshoption/)
* class [PivotCache](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Refresh() {#refresh}

Aktualisiert Daten aus der Datenquelle und berechnet Daten für die Ansicht aller Pivot-Tabellen, deren Datenquelle dieser Pivot-Cache ist.

```csharp
public PivotRefreshState Refresh()
```

### Hinweise

Wenn sowohl table1 als auch table2 diesen Cache verwenden, werden die beiden Tabellen berechnet. Es ist besser, wenn Sie einfach [`RefreshAll`](../../../aspose.cells/workbook/refreshall/) aufrufen, um alle PivotTables und Diagramme in der Datei zu aktualisieren.

### Siehe auch

* enum [PivotRefreshState](../../pivotrefreshstate/)
* class [PivotCache](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


