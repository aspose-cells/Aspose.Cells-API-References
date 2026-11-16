---
title: "PivotCache Klasse"
linktitle: "PivotCache"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "PivotCache-Klasse. Kapselt das Objekt, das pivotcache in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/pivotcache/
---

## PivotCache class

Stellt den Speicher-Cache für einige PivotTable-Berichte dar.

```go

type PivotCache struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetMissingItemsLimit](./getmissingitemslimit/) | Liest und setzt die Anzahl nicht verwendeter Elemente, die erlaubt sind, bevor nicht verwendete Elemente verworfen werden. Dieser Wert MUSS größer als -2 und kleiner als 1048577.PivotCacheMissingItemsLimitConst; |
| [SetMissingItemsLimit](./setmissingitemslimit/) | Liest und setzt die Anzahl nicht verwendeter Elemente, die erlaubt sind, bevor nicht verwendete Elemente verworfen werden. Dieser Wert MUSS größer als -2 und kleiner als 1048577.PivotCacheMissingItemsLimitConst; |
| [Refresh_PivotTableRefreshOption](./refresh_pivottablerefreshoption/) | Aktualisiert Daten aus der Datenquelle und berechnet Daten für die Ansicht aller Pivot-Tabellen, deren Datenquelle dieser Pivot-Cache ist. |
| [Refresh](./refresh/) | Aktualisiert Daten aus der Datenquelle und berechnet Daten für die Ansicht aller Pivot-Tabellen, deren Datenquelle dieser Pivot-Cache ist. |
| [GetPivotTables](./getpivottables/) | Liest alle Pivot-Tabellen mit diesem Pivot-Cache. |
| [Dispose](./dispose/) | Gibt alle Ressourcen frei. |
| [GetSourceType](./getsourcetype/) | Liest den PivotTableSourceType. |
