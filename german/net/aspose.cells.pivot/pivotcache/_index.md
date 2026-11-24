---
title: "Klasse PivotCache"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Pivot.PivotCache Klasse. Stellt den Speicher-Cache für einige PivotTable-Berichte dar"
type: docs
url: /de/net/aspose.cells.pivot/pivotcache/
---
## PivotCache class

Stellt den Speicher-Cache für einige PivotTable-Berichte dar.

```csharp
public abstract class PivotCache : IDisposable
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [MissingItemsLimit](../../aspose.cells.pivot/pivotcache/missingitemslimit/) { get; set; } | Liest und setzt die Anzahl nicht verwendeter Elemente, die zulässig sind, bevor nicht verwendete Elemente verworfen werden. Dieser Wert MUSS größer als -2 und kleiner als 1048577 sein. [`PivotCacheMissingItemsLimitConst`](../pivotcachemissingitemslimitconst/); |
| abstract [SourceType](../../aspose.cells.pivot/pivotcache/sourcetype/) { get; } | Liest den [`PivotTableSourceType`](../pivottablesourcetype/). |

## Methoden

| Name | Beschreibung |
| --- | --- |
| abstract [Dispose](../../aspose.cells.pivot/pivotcache/dispose/)() | Alle Ressourcen freigeben. |
| [GetPivotTables](../../aspose.cells.pivot/pivotcache/getpivottables/)() | Liest alle Pivot-Tabellen mit diesem Pivot-Cache. |
| [Refresh](../../aspose.cells.pivot/pivotcache/refresh/#refresh)() | Aktualisiert Daten aus der Datenquelle und berechnet Daten für die Ansicht aller Pivot-Tabellen, deren Datenquelle dieser Pivot-Cache ist. |
| [Refresh](../../aspose.cells.pivot/pivotcache/refresh/#refresh_1)(PivotTableRefreshOption) | Aktualisiert Daten aus der Datenquelle und berechnet Daten für die Ansicht aller Pivot-Tabellen, deren Datenquelle dieser Pivot-Cache ist. |

### Hinweise

Alle Daten werden in diesen Cache gesammelt, und die Pivot-Tabelle erhält Daten nur aus diesem Cache, nicht direkt aus der Datenquelle. Wenn die Datenquelle einiger [`PivotTable`](../pivottable/)s gleich ist, verwenden sie einen Pivot-Cache.

### Siehe auch

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


