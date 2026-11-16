---
title: "DataBar Klasse"
linktitle: "DataBar"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "DataBar Klasse. Kapselt das Objekt, das databar in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/databar/
---

## DataBar class

Beschreibt die DataBar‑Bedingte-Formatierungsregel. Diese bedingte Formatierungsregel zeigt eine abgestufte Datenleiste im Zellbereich an.

```go

type DataBar struct  {
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
| [GetAxisColor](./getaxiscolor/) | Ruft die Farbe der Achse für Zellen mit bedingter Formatierung als Datenbalken ab. |
| [SetAxisColor](./setaxiscolor/) | Ruft die Farbe der Achse für Zellen mit bedingter Formatierung als Datenbalken ab. |
| [GetAxisPosition](./getaxisposition/) | Liest oder setzt die Position der Achse der Datenbalken, die durch eine Regel für bedingte Formatierung angegeben ist. |
| [SetAxisPosition](./setaxisposition/) | Liest oder setzt die Position der Achse der Datenbalken, die durch eine Regel für bedingte Formatierung angegeben ist. |
| [GetBarFillType](./getbarfilltype/) | Liest oder setzt, wie ein Datenbalken mit Farbe gefüllt wird. |
| [SetBarFillType](./setbarfilltype/) | Liest oder setzt, wie ein Datenbalken mit Farbe gefüllt wird. |
| [GetDirection](./getdirection/) | Liest oder setzt die Richtung, in der der Datenbalken angezeigt wird. |
| [SetDirection](./setdirection/) | Liest oder setzt die Richtung, in der der Datenbalken angezeigt wird. |
| [GetBarBorder](./getbarborder/) | Ruft ein Objekt ab, das den Rand eines Datenbalkens festlegt. |
| [GetNegativeBarFormat](./getnegativebarformat/) | Ruft das NegativeBarFormat‑Objekt ab, das mit einer Regel für bedingte Formatierung eines Datenbalkens verknüpft ist. |
| [GetMinCfvo](./getmincfvo/) | Rufe oder setze das Minimalwert‑Objekt dieses DataBar. Null oder ein CFValueObject vom Typ FormatConditionValueType.Max kann nicht zugewiesen werden. |
| [GetMaxCfvo](./getmaxcfvo/) | Rufe oder setze das Maximalwert‑Objekt dieses DataBar. Null oder ein CFValueObject vom Typ FormatConditionValueType.Min kann nicht zugewiesen werden. |
| [GetColor](./getcolor/) | Rufe oder setze die Farbe dieses DataBar. |
| [SetColor](./setcolor/) | Rufe oder setze die Farbe dieses DataBar. |
| [GetMinLength](./getminlength/) | Stellt die minimale Länge der Datenleiste dar. |
| [SetMinLength](./setminlength/) | Stellt die minimale Länge der Datenleiste dar. |
| [GetMaxLength](./getmaxlength/) | Stellt die maximale Länge der Datenleiste dar. |
| [SetMaxLength](./setmaxlength/) | Stellt die maximale Länge der Datenleiste dar. |
| [GetShowValue](./getshowvalue/) | Lese oder setze das Flag, das angibt, ob die Werte der Zellen, auf die diese Datenleiste angewendet wird, angezeigt werden sollen. Der Standardwert ist true. |
| [SetShowValue](./setshowvalue/) | Lese oder setze das Flag, das angibt, ob die Werte der Zellen, auf die diese Datenleiste angewendet wird, angezeigt werden sollen. Der Standardwert ist true. |
| [ToImage](./toimage/) | Rendere die Datenleiste in einer Zelle zu einem Bild-Byte-Array. |
