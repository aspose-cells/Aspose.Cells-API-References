---
title: "AutoFilter Klasse"
linktitle: "AutoFilter"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "AutoFilter Klasse. Kapselt das Objekt, das autofilter in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/autofilter/
---

## AutoFilter class

Stellt die Autofilterung für das angegebene Arbeitsblatt dar.

```go

type AutoFilter struct  {
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
| [GetSorter](./getsorter/) | Liest den Datensortierer. |
| [SetRange_Int_Int_Int](./setrange_int_int_int/) | Setzt den Bereich, auf den der angegebene AutoFilter angewendet wird. |
| [GetCellArea](./getcellarea/) | Liest den CellArea, auf den dieser AutoFilter angewendet wird. |
| [GetCellArea_Bool](./getcellarea_bool/) | Liest den Aspose.Cells.CellArea, auf den der angegebene AutoFilter angewendet wird. |
| [GetRange](./getrange/) | Stellt den Bereich dar, auf den der angegebene AutoFilter angewendet wird. |
| [SetRange_String](./setrange_string/) | Stellt den Bereich dar, auf den der angegebene AutoFilter angewendet wird. |
| [AddFilter](./addfilter/) | Fügt einen Filter für eine Filterspalte hinzu. |
| [AddDateFilter](./adddatefilter/) | Fügt einen Datumsfilter hinzu. |
| [RemoveDateFilter](./removedatefilter/) | Entfernt einen Datumsfilter. |
| [RemoveFilter_Int_String](./removefilter_int_string/) | Entfernt einen Filter für eine Filterspalte. |
| [Filter](./filter/) | Filtert eine Liste mit angegebenen Kriterien. |
| [FilterTop10](./filtertop10/) | Filtere die Top‑10‑Elemente in der Liste |
| [Dynamic_Filter](./dynamic_filter/) | Fügt einen dynamischen Filter hinzu. |
| [AddFontColorFilter](./addfontcolorfilter/) | Fügt einen Schriftfarbenfilter hinzu. |
| [AddFillColorFilter](./addfillcolorfilter/) | Fügt einen Füllfarbenfilter hinzu. |
| [AddIconFilter](./addiconfilter/) | Fügt einen Symbolfilter hinzu. |
| [MatchBlanks](./matchblanks/) | Alle leeren Zellen in der Liste abgleichen. |
| [MatchNonBlanks](./matchnonblanks/) | Alle nicht-leeren Zellen in der Liste abgleichen. |
| [Custom_Int_FilterOperatorType_Object](./custom_int_filteroperatortype_object/) | Filtert eine Liste mit einem benutzerdefinierten Kriterium. |
| [Custom_Int_FilterOperatorType_Object_Bool_FilterOperatorType_Object](./custom_int_filteroperatortype_object_bool_filteroperatortype_object/) | Filtert eine Liste mit benutzerdefinierten Kriterien. |
| [ShowAll](./showall/) | Alle Zeilen einblenden. |
| [RemoveFilter_Int](./removefilter_int/) | Entferne den spezifischen Filter. |
| [Refresh](./refresh/) | Aktualisiere die Auto‑Filter, um die Zeilen auszublenden oder einzublenden. |
| [Refresh_Bool](./refresh_bool/) | Ermittelt die Indizes aller ausgeblendeten Zeilen. |
| [GetShowFilterButton](./getshowfilterbutton/) | Gibt an, ob die AutoFilter‑Schaltfläche für diese Spalte sichtbar ist. |
| [SetShowFilterButton](./setshowfilterbutton/) | Gibt an, ob die AutoFilter‑Schaltfläche für diese Spalte sichtbar ist. |
| [GetFilterColumns](./getfiltercolumns/) | Ermittelt die Sammlung der Filterspalten. |
