---
title: "ConditionalFormattingValue-Klasse"
linktitle: "ConditionalFormattingValue"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "ConditionalFormattingValue-Klasse. Kapselt das Objekt, das conditionalformattingvalue in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/conditionalformattingvalue/
---

## ConditionalFormattingValue class

Beschreibt die Werte der Interpolationspunkte in einer Farbskala, Datenleiste oder Symbolsatz.

```go

type ConditionalFormattingValue struct  {
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
| [GetValue](./getvalue/) | Lese oder setze den Wert dieses Conditional-Formatting-Wertobjekts. Es sollte zusammen mit Type verwendet werden. |
| [SetValue](./setvalue/) | Lese oder setze den Wert dieses Conditional-Formatting-Wertobjekts. Es sollte zusammen mit Type verwendet werden. |
| [GetType](./gettype/) | Lese oder setze den Typ dieses Conditional-Formatting-Wertobjekts. Das Setzen des Typs auf FormatConditionValueType.Min oder FormatConditionValueType.Max setzt "Value" automatisch auf null. |
| [SetType](./settype/) | Lese oder setze den Typ dieses Conditional-Formatting-Wertobjekts. Das Setzen des Typs auf FormatConditionValueType.Min oder FormatConditionValueType.Max setzt "Value" automatisch auf null. |
| [IsGTE](./isgte/) | Abrufen oder Festlegen des Greater Than Or Equal-Flags. Nur für Symbolsets verwenden, bestimmt, ob dieser Schwellenwert den Größer‑als‑oder‑gleich‑Operator verwendet. 'false' bedeutet, dass 'greater than' anstelle von 'greater than or equal to' verwendet wird. Standardwert ist true. |
| [SetIsGTE](./setisgte/) | Abrufen oder Festlegen des Greater Than Or Equal-Flags. Nur für Symbolsets verwenden, bestimmt, ob dieser Schwellenwert den Größer‑als‑oder‑gleich‑Operator verwendet. 'false' bedeutet, dass 'greater than' anstelle von 'greater than or equal to' verwendet wird. Standardwert ist true. |
