---
title: "PivotTableCollection Klasse"
linktitle: "PivotTableCollection"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "PivotTableCollection Klasse. Kapselt das Objekt, das pivottablecollection in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/pivottablecollection/
---

## PivotTableCollection class

Stellt die Sammlung aller PivotTable‑Objekte im angegebenen Arbeitsblatt dar.

```go

type PivotTableCollection struct  {
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
| [Dispose](./dispose/) | Führt anwendungsspezifische Aufgaben aus, die mit dem Freigeben, Freisetzen oder Zurücksetzen nicht verwalteter Ressourcen verbunden sind. |
| [Add_String_Int_Int](./add_string_int_int/) | Fügt eine neue PivotTable an der angegebenen Zeilen- und Spaltenposition des Arbeitsblatts mit Standardoptionen hinzu. |
| [Add_String_Int_Int_String_Bool_Bool](./add_string_int_int_string_bool_bool/) | Fügt eine neue PivotTable mit dem Legacy-Layout und -Stil von Excel 97-2003 hinzu. |
| [Add_String_String_String_Bool_Bool](./add_string_string_string_bool_bool/) | Fügt eine neue PivotTable hinzu. |
| [Add_PivotTable_String_String](./add_pivottable_string_string/) | Fügt eine neue PivotTable basierend auf einer anderen PivotTable hinzu. |
| [Add_PivotTable_Int_Int_String](./add_pivottable_int_int_string/) | Fügt eine neue PivotTable basierend auf einer anderen PivotTable hinzu. |
| [Add_stringArray_Bool_PivotPageFields_String_String](./add_stringarray_bool_pivotpagefields_string_string/) | Fügt ein neues PivotTable-Objekt zur Sammlung hinzu, wobei mehrere Konsolidierungsbereiche als Datenquelle verwendet werden. |
| [Add_stringArray_Bool_PivotPageFields_Int_Int_String](./add_stringarray_bool_pivotpagefields_int_int_string/) | Fügt ein neues PivotTable-Objekt zur Sammlung hinzu, wobei mehrere Konsolidierungsbereiche als Datenquelle verwendet werden. |
| [Get_Int](./get_int/) | Liefert den PivotTable-Bericht nach Index. |
| [Get_String](./get_string/) | Liefert den PivotTable-Bericht nach dem Namen der PivotTable. |
| [Get_Int_Int](./get_int_int/) | Liefert den PivotTable-Bericht nach der Position der PivotTable. |
| [Clear](./clear/) | Löscht alle PivotTables. |
| [Remove_PivotTable](./remove_pivottable/) | Löscht die angegebene PivotTable und entfernt die PivotTable-Daten. |
| [Remove_PivotTable_Bool](./remove_pivottable_bool/) | Löscht die angegebene PivotTable. |
| [RemoveAt_Int](./removeat_int/) | Löscht die PivotTable am angegebenen Index und entfernt die PivotTable-Daten. |
| [RemoveAt_Int_Bool](./removeat_int_bool/) | Löscht die PivotTable am angegebenen Index. |
| [GetCount](./getcount/) | Liefert die Anzahl der im Objekt enthaltenen Elemente. |
