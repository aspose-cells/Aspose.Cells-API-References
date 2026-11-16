---
title: "PivotFieldCollection-Klasse"
linktitle: "PivotFieldCollection"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "PivotFieldCollection-Klasse. Kapselt das Objekt, das die PivotFieldCollection in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/pivotfieldcollection/
---

## PivotFieldCollection class

Stellt eine Sammlung aller PivotField‑Objekte in den verschiedenen Bereichen der Pivot‑Tabelle dar.

```go

type PivotFieldCollection struct  {
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
| [GetType](./gettype/) | Gibt den Typ PivotFields zurück. |
| [Get_Int](./get_int/) | Gibt das PivotField-Objekt am angegebenen Index zurück. |
| [Get_String](./get_string/) | Gibt das PivotField-Objekt mit dem angegebenen Namen zurück. |
| [RemoveAt](./removeat/) | Entfernt das Feld nach Index. Nur für Filter-, Zeilen-, Spalten- und Datenbereich. |
| [AddByBaseIndex](./addbybaseindex/) | Fügt ein PivotField-Objekt zum angegebenen Typ PivotFields hinzu. |
| [Add](./add/) | Fügt ein PivotField-Objekt zum angegebenen Typ PivotFields hinzu. |
| [Insert](./insert/) | Fügt ein Pivot-Feld an einem bestimmten Index ein. |
| [Clear](./clear/) | Alle Felder der PivotFieldCollection löschen |
| [Remove](./remove/) | Entfernt das Feld aus dem aktuellen Bereich. |
| [Move](./move/) | Verschiebt das PivotField von der aktuellen Position zur Zielposition. |
| [GetCount](./getcount/) | Liefert die Anzahl der im Objekt enthaltenen Elemente. |
