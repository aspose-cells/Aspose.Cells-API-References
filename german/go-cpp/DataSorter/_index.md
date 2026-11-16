---
title: "DataSorter Klasse"
linktitle: "DataSorter"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "DataSorter Klasse. Kapselt das Objekt, das DataSorter in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/datasorter/
---

## DataSorter class

Zusammenfassende Beschreibung für DataSorter.

```go

type DataSorter struct  {
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
| [GetKeys](./getkeys/) | Ermittelt die Schlüsselliste des DataSorters. |
| [Clear](./clear/) | Alle Einstellungen zurücksetzen. |
| [GetHasHeaders](./gethasheaders/) | Gibt an, ob der Bereich Überschriften enthält. |
| [SetHasHeaders](./sethasheaders/) | Gibt an, ob der Bereich Überschriften enthält. |
| [AddKey_Int_SortOrder](./addkey_int_sortorder/) | Fügt sortierten Spaltenindex und Sortierreihenfolge hinzu. |
| [AddKey_Int_SortOrder_String](./addkey_int_sortorder_string/) | Fügt sortierten Spaltenindex und Sortierreihenfolge mit benutzerdefinierter Sortierliste hinzu. |
| [AddColorKey](./addcolorkey/) | Fügt Farbsortierschlüssel hinzu. |
| [AddKey_Int_SortOnType_SortOrder_Object](./addkey_int_sortontype_sortorder_object/) | Fügt sortierten Spaltenindex und Sortierreihenfolge mit benutzerdefinierter Sortierliste hinzu. |
| [AddKey_Int_SortOrder_stringArray](./addkey_int_sortorder_stringarray/) | Fügt sortierten Spaltenindex und Sortierreihenfolge mit benutzerdefinierter Sortierliste hinzu. |
| [GetKey1](./getkey1/) | Gibt den ersten sortierten Spaltenindex an (absolute Position, Spalte A ist 0, B ist 1, ...). |
| [SetKey1](./setkey1/) | Gibt den ersten sortierten Spaltenindex an (absolute Position, Spalte A ist 0, B ist 1, ...). |
| [GetOrder1](./getorder1/) | Gibt die Sortierreihenfolge des ersten Schlüssels an. |
| [SetOrder1](./setorder1/) | Gibt die Sortierreihenfolge des ersten Schlüssels an. |
| [GetKey2](./getkey2/) | Gibt den zweiten sortierten Spaltenindex an (absolute Position, Spalte A ist 0, B ist 1, ...). |
| [SetKey2](./setkey2/) | Gibt den zweiten sortierten Spaltenindex an (absolute Position, Spalte A ist 0, B ist 1, ...). |
| [GetOrder2](./getorder2/) | Gibt die Sortierreihenfolge des zweiten Schlüssels an. |
| [SetOrder2](./setorder2/) | Gibt die Sortierreihenfolge des zweiten Schlüssels an. |
| [GetKey3](./getkey3/) | Gibt den dritten sortierten Spaltenindex an (absolute Position, Spalte A ist 0, B ist 1, ...). |
| [SetKey3](./setkey3/) | Gibt den dritten sortierten Spaltenindex an (absolute Position, Spalte A ist 0, B ist 1, ...). |
| [GetOrder3](./getorder3/) | Stellt die Sortierreihenfolge des dritten Schlüssels dar. |
| [SetOrder3](./setorder3/) | Stellt die Sortierreihenfolge des dritten Schlüssels dar. |
| [GetSortLeftToRight](./getsortlefttoright/) | True bedeutet, dass die Sortierrichtung von links nach rechts ist.False bedeutet, dass die Sortierrichtung von oben nach unten ist.Der Standardwert ist false. |
| [SetSortLeftToRight](./setsortlefttoright/) | True bedeutet, dass die Sortierrichtung von links nach rechts ist.False bedeutet, dass die Sortierrichtung von oben nach unten ist.Der Standardwert ist false. |
| [GetCaseSensitive](./getcasesensitive/) | Liest und setzt, ob bei Zeichenkettenvergleich die Groß-/Kleinschreibung berücksichtigt wird. |
| [SetCaseSensitive](./setcasesensitive/) | Liest und setzt, ob bei Zeichenkettenvergleich die Groß-/Kleinschreibung berücksichtigt wird. |
| [GetSortAsNumber](./getsortasnumber/) | Gibt an, ob alles, was wie eine Zahl aussieht, sortiert wird. |
| [SetSortAsNumber](./setsortasnumber/) | Gibt an, ob alles, was wie eine Zahl aussieht, sortiert wird. |
| [Sort_Cells_Int_Int_Int_Int](./sort_cells_int_int_int_int/) | Sortiert die Daten des Bereichs. |
| [Sort_Cells_CellArea](./sort_cells_cellarea/) | Sortiere die Daten des Bereichs. |
| [Sort](./sort/) | Sortiere die Daten im Bereich. |
