---
title: "PivotAreaFilter Klasse"
linktitle: "PivotAreaFilter"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "PivotAreaFilter Klasse. Kapselt das Objekt, das pivotareafilter in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/pivotareafilter/
---

## PivotAreaFilter class

Stellt den Filter von <see cref="PivotArea"/> für <see cref="PivotTable"/> dar.

```go

type PivotAreaFilter struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewPivotAreaFilter](./newpivotareafilter/) | Standardkonstruktor. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [IsSubtotalSet](./issubtotalset/) | Ermittelt, welcher Zwischensumme für diesen Filter festgelegt ist. |
| [SetSubtotals](./setsubtotals/) | Zwischensumme für den Filter. |
| [GetFieldIndex](./getfieldindex/) | Ermittelt den Index des Feldes in den Quellfeldern, auf das sich dieser Filter bezieht. Ein Wert von -2 zeigt das Wertefeld an. |
| [GetSelected](./getselected/) | Gibt an, ob dieses Feld eine Auswahl hat. Funktioniert nur, wenn die PivotTable in der Gliederungsansicht ist. |
| [SetSelected](./setselected/) | Gibt an, ob dieses Feld eine Auswahl hat. Funktioniert nur, wenn die PivotTable in der Gliederungsansicht ist. |
