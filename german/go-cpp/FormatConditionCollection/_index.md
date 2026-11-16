---
title: "FormatConditionCollection Klasse"
linktitle: "FormatConditionCollection"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "FormatConditionCollection Klasse. Kapselt das Objekt, das formatconditioncollection in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/formatconditioncollection/
---

## FormatConditionCollection class

Stellt bedingte Formatierung dar. Die FormatConditions können bis zu drei bedingte Formate enthalten.

```go

type FormatConditionCollection struct  {
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
| [Add](./add/) | Fügt eine Formatierungsbedingung und den betroffenen Zellbereich zu den FormatConditions hinzu. Die FormatConditions können bis zu drei bedingte Formate enthalten. Verweise auf andere Tabellenblätter sind in den Formeln der bedingten Formatierung nicht zulässig. |
| [AddArea](./addarea/) | Fügt einen bedingt formatierten Zellbereich hinzu. |
| [AddCondition_FormatConditionType_OperatorType_String_String](./addcondition_formatconditiontype_operatortype_string_string/) | Fügt eine Formatierungsbedingung hinzu. |
| [AddCondition_FormatConditionType](./addcondition_formatconditiontype/) | Füge eine Formatbedingung hinzu. |
| [GetCount](./getcount/) | Gibt die Anzahl der Bedingungen zurück. |
| [GetRangeCount](./getrangecount/) | Ermittelt die Anzahl der bedingt formatierten Bereiche. |
| [Get](./get/) | Ermittelt die Formatierungsbedingung nach Index. |
| [GetCellArea](./getcellarea/) | Ermittelt den bedingt formatierten Zellbereich nach Index. |
| [RemoveArea_Int](./removearea_int/) | Entfernt den bedingt formatierten Zellbereich nach Index. |
| [RemoveArea_Int_Int_Int_Int](./removearea_int_int_int_int/) | Entfernt die bedingte Formatierung im Bereich. |
| [RemoveCondition](./removecondition/) | Entfernt die Formatierungsbedingung nach Index. |
