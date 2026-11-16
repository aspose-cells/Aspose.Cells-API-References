---
title: "ColorScale Klasse"
linktitle: "ColorScale"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "ColorScale Klasse. Kapselt das Objekt, das colorscale in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/colorscale/
---

## ColorScale class

Beschreibt die ColorScale‑Bedingte-Formatierungsregel. Diese bedingte Formatierungsregel erstellt eine abgestufte Farbskala in den Zellen.

```go

type ColorScale struct  {
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
| [GetIs3ColorScale](./getis3colorscale/) | Gibt an, ob die bedingte Formatierung eine 3‑Farben‑Skala ist. |
| [SetIs3ColorScale](./setis3colorscale/) | Gibt an, ob die bedingte Formatierung eine 3‑Farben‑Skala ist. |
| [GetMinCfvo](./getmincfvo/) | Lese oder setze das Minimalwert‑Objekt dieser ColorScale. Null oder ein CFValueObject mit dem Typ FormatConditionValueType.Max kann nicht zugewiesen werden. |
| [GetMidCfvo](./getmidcfvo/) | Lese oder setze das Mittelwert‑Objekt dieser ColorScale. Ein CFValueObject mit dem Typ FormatConditionValueType.Max oder FormatConditionValueType.Min kann nicht zugewiesen werden. |
| [GetMaxCfvo](./getmaxcfvo/) | Lese oder setze das Maximalwert‑Objekt dieser ColorScale. Null oder ein CFValueObject mit dem Typ FormatConditionValueType.Min kann nicht zugewiesen werden. |
| [GetMinColor](./getmincolor/) | Lese oder setze die Farbverlauffarbe für den Minimalwert im Bereich. |
| [SetMinColor](./setmincolor/) | Lese oder setze die Farbverlauffarbe für den Minimalwert im Bereich. |
| [GetMidColor](./getmidcolor/) | Lese oder setze die Farbverlauffarbe für den Mittelwert im Bereich. |
| [SetMidColor](./setmidcolor/) | Lese oder setze die Farbverlauffarbe für den Mittelwert im Bereich. |
| [GetMaxColor](./getmaxcolor/) | Lese oder setze die Farbverlauffarbe für den Maximalwert im Bereich. |
| [SetMaxColor](./setmaxcolor/) | Lese oder setze die Farbverlauffarbe für den Maximalwert im Bereich. |
