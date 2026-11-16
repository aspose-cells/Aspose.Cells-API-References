---
title: "SeriesCollection Klasse"
linktitle: "SeriesCollection"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "SeriesCollection Klasse. Kapselt das Objekt, das die SeriesCollection in Go repräsentiert."
type: docs
weight: 200
url: /de/go-cpp/seriescollection/
---

## SeriesCollection class

Kapselt eine Sammlung von <see cref=\"Series\"/>-Objekten.

```go

type SeriesCollection struct  {
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
| [Get](./get/) | Liest das Series-Element am angegebenen Index. |
| [GetSeriesByOrder](./getseriesbyorder/) | Ruft das Series-Element nach Reihenfolge ab. |
| [RemoveAt](./removeat/) | Entfernt eine Serie am spezifischen Index. |
| [GetCategoryData](./getcategorydata/) | Liest oder setzt den Bereich der Kategorien-Achsenwerte. Es kann ein Zellbereich sein (z. B. "d1:e10") oder eine Wertefolge (z. B. "{2,6,8,10}"). |
| [SetCategoryData](./setcategorydata/) | Liest oder setzt den Bereich der Kategorien-Achsenwerte. Es kann ein Zellbereich sein (z. B. "d1:e10") oder eine Wertefolge (z. B. "{2,6,8,10}"). |
| [GetSecondCategoryData](./getsecondcategorydata/) | Liest oder setzt den Bereich der zweiten Kategorien-Achsenwerte. Es kann ein Zellbereich sein (z. B. "d1:e10"), oder eine Wertefolge (z. B. "{2,6,8,10}"). Wirkt nur, wenn einige Serien auf der zweiten Achse dargestellt wurden. |
| [SetSecondCategoryData](./setsecondcategorydata/) | Liest oder setzt den Bereich der zweiten Kategorien-Achsenwerte. Es kann ein Zellbereich sein (z. B. "d1:e10"), oder eine Wertefolge (z. B. "{2,6,8,10}"). Wirkt nur, wenn einige Serien auf der zweiten Achse dargestellt wurden. |
| [SwapSeries](./swapseries/) | Ändert direkt die Reihenfolge der beiden Serien. |
| [SetSeriesNames](./setseriesnames/) | Setzt die Namen aller Serien im Diagramm. |
| [AddR1C1](./addr1c1/) | Fügt die Series-Sammlung zu einem Diagramm hinzu. |
| [Add_String_Bool](./add_string_bool/) | Fügt die Series-Sammlung zu einem Diagramm hinzu. |
| [Add_String_Bool_Bool](./add_string_bool_bool/) | Fügt die Series-Sammlung zu einem Diagramm hinzu. |
| [IsColorVaried](./iscolorvaried/) | Gibt an, ob die Farbe der Punkte variiert wird. |
| [SetIsColorVaried](./setiscolorvaried/) | Gibt an, ob die Farbe der Punkte variiert wird. |
| [Clear](./clear/) | Leert die Sammlung |
| [ChangeColors](./changecolors/) | Setzt eine monochrome Palette für Diagramm-Serien. |
| [GetCount](./getcount/) | Liefert die Anzahl der im Objekt enthaltenen Elemente. |
