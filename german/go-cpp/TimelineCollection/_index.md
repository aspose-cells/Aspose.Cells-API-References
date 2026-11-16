---
title: "TimelineCollection Klasse"
linktitle: "TimelineCollection"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "TimelineCollection Klasse. Kapselt das Objekt, das timelinecollection in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/timelinecollection/
---

## TimelineCollection class

Gibt die Sammlung aller <see cref="Timeline"/>-Objekte im Arbeitsblatt an. Es wird seit Excel 2013 unterstützt.

```go

type TimelineCollection struct  {
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
| [Get_Int](./get_int/) | Ruft die Timeline nach Index ab. |
| [Get_String](./get_string/) | Ruft die Timeline nach dem Namen der Timeline ab. |
| [Add_PivotTable_Int_Int_String](./add_pivottable_int_int_string/) | Fügt eine neue Timeline hinzu, die PivotTable als Datenquelle verwendet. |
| [Add_PivotTable_String_String](./add_pivottable_string_string/) | Fügt eine neue Timeline hinzu, die PivotTable als Datenquelle verwendet. |
| [Add_PivotTable_Int_Int_Int](./add_pivottable_int_int_int/) | Fügt eine neue Timeline hinzu, die PivotTable als Datenquelle verwendet. |
| [Add_PivotTable_String_Int](./add_pivottable_string_int/) | Fügt eine neue Timeline hinzu, die PivotTable als Datenquelle verwendet. |
| [Add_PivotTable_Int_Int_PivotField](./add_pivottable_int_int_pivotfield/) | Fügt eine neue Timeline hinzu, die PivotTable als Datenquelle verwendet. |
| [Add_PivotTable_String_PivotField](./add_pivottable_string_pivotfield/) | Fügt eine neue Timeline hinzu, die PivotTable als Datenquelle verwendet. |
| [GetCount](./getcount/) | Liefert die Anzahl der im Objekt enthaltenen Elemente. |
