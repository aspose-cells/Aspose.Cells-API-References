---
title: "Top10 Klasse"
linktitle: "Top10"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "Top10 Klasse. Kapselt das Objekt, das top10 in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/top10/
---

## Top10 class

Beschreiben Sie die Top10 bedingte Formatierungsregel.Diese bedingte Formatierungsregel hebt Zellen hervor, deren Werte in den oberen N‑ oder unteren N‑Bereich fallen, wie angegeben.

```go

type Top10 struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewTop10](./newtop10/) | Standardkonstruktor. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [IsPercent](./ispercent/) | Lese oder setze, ob eine "top/bottom n"-Regel eine "top/bottom n Prozent"-Regel ist. Standardwert ist false. |
| [SetIsPercent](./setispercent/) | Lese oder setze, ob eine "top/bottom n"-Regel eine "top/bottom n Prozent"-Regel ist. Standardwert ist false. |
| [IsBottom](./isbottom/) | Lese oder setze, ob eine "top/bottom n"-Regel eine "bottom n"-Regel ist. Standardwert ist false. |
| [SetIsBottom](./setisbottom/) | Lese oder setze, ob eine "top/bottom n"-Regel eine "bottom n"-Regel ist. Standardwert ist false. |
| [GetRank](./getrank/) | Lese oder setze den Wert von "n" in einer "top/bottom n"-bedingten Formatierungsregel. Wenn IsPercent true ist, muss der Wert zwischen 0 und 100 liegen. Andernfalls muss er zwischen 0 und 1000 liegen. Standardwert ist 10. |
| [SetRank](./setrank/) | Lese oder setze den Wert von "n" in einer "top/bottom n"-bedingten Formatierungsregel. Wenn IsPercent true ist, muss der Wert zwischen 0 und 100 liegen. Andernfalls muss er zwischen 0 und 1000 liegen. Standardwert ist 10. |
