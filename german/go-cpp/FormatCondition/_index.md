---
title: "FormatCondition Klasse"
linktitle: "FormatCondition"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "FormatCondition Klasse. Kapselt das Objekt, das formatcondition in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/formatcondition/
---

## FormatCondition class

Stellt eine bedingte Formatierungsbedingung dar.

```go

type FormatCondition struct  {
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
| [GetFormula1_Bool_Bool](./getformula1_bool_bool/) | Liefert den Wert oder Ausdruck, der mit dieser Formatbedingung verknüpft ist. |
| [GetFormula2_Bool_Bool](./getformula2_bool_bool/) | Liefert den Wert oder Ausdruck, der mit dieser Formatbedingung verknüpft ist. |
| [GetFormula1_Bool_Bool_Int_Int](./getformula1_bool_bool_int_int/) | Liefert den Wert oder Ausdruck der bedingten Formatierung der Zelle. |
| [GetFormula2_Bool_Bool_Int_Int](./getformula2_bool_bool_int_int/) | Liefert den Wert oder Ausdruck der bedingten Formatierung der Zelle. |
| [SetFormulas](./setformulas/) | Setzt den Wert oder Ausdruck, der mit dieser Formatbedingung verknüpft ist. |
| [SetFormula1_String_Bool_Bool](./setformula1_string_bool_bool/) | Setzt den Wert oder Ausdruck, der mit dieser Formatbedingung verknüpft ist. |
| [SetFormula2_String_Bool_Bool](./setformula2_string_bool_bool/) | Setzt den Wert oder Ausdruck, der mit dieser Formatbedingung verknüpft ist. |
| [GetFormula1](./getformula1/) | Liest und setzt den Wert oder Ausdruck, der mit der bedingten Formatierung verknüpft ist. |
| [SetFormula1_String](./setformula1_string/) | Liest und setzt den Wert oder Ausdruck, der mit der bedingten Formatierung verknüpft ist. |
| [GetFormula1_Int_Int](./getformula1_int_int/) | Liefert die Formel der bedingten Formatierung der Zelle. |
| [GetFormula2](./getformula2/) | Liest und setzt den Wert oder Ausdruck, der mit der bedingten Formatierung verknüpft ist. |
| [SetFormula2_String](./setformula2_string/) | Liest und setzt den Wert oder Ausdruck, der mit der bedingten Formatierung verknüpft ist. |
| [GetFormula2_Int_Int](./getformula2_int_int/) | Liefert die Formel der bedingten Formatierung der Zelle. |
| [GetOperator](./getoperator/) | Liest und setzt den Operatortyp der bedingten Formatierung. |
| [SetOperator](./setoperator/) | Liest und setzt den Operatortyp der bedingten Formatierung. |
| [GetStopIfTrue](./getstopiftrue/) | Wahr, keine Regeln mit niedrigerer Priorität dürfen über dieser Regel angewendet werden, wenn diese Regel zu wahr evaluiert wird.Gilt nur für Excel 2007; |
| [SetStopIfTrue](./setstopiftrue/) | Wahr, keine Regeln mit niedrigerer Priorität dürfen über dieser Regel angewendet werden, wenn diese Regel zu wahr evaluiert wird.Gilt nur für Excel 2007; |
| [GetPriority](./getpriority/) | Die Priorität dieser bedingten Formatierungsregel. Dieser Wert wird verwendet, um zu bestimmen, welchesformat ausgewertet und gerendert werden soll. Niedrigere numerische Werte haben höhere Priorität alshöhere numerische Werte, wobei '1' die höchste Priorität hat. |
| [SetPriority](./setpriority/) | Die Priorität dieser bedingten Formatierungsregel. Dieser Wert wird verwendet, um zu bestimmen, welchesformat ausgewertet und gerendert werden soll. Niedrigere numerische Werte haben höhere Priorität alshöhere numerische Werte, wobei '1' die höchste Priorität hat. |
| [GetStyle](./getstyle/) | Liest oder setzt den Stil von bedingt formatierten Zellbereichen. |
| [SetStyle](./setstyle/) | Liest oder setzt den Stil von bedingt formatierten Zellbereichen. |
| [GetType](./gettype/) | Liest und schreibt, ob der bedingte Formattyp verwendet wird. |
| [SetType](./settype/) | Liest und schreibt, ob der bedingte Formattyp verwendet wird. |
| [GetIconSet](./geticonset/) | Gibt die "IconSet"-Instanz der bedingten Formatierung zurück. Der Standardinstanz-IconSetType ist TrafficLights31. Gültig nur für type = IconSet. |
| [GetDataBar](./getdatabar/) | Gibt die "DataBar"-Instanz der bedingten Formatierung zurück. Die Standardinstanzfarbe ist blau. Gültig nur für type ist DataBar. |
| [GetColorScale](./getcolorscale/) | Gibt die "ColorScale"-Instanz der bedingten Formatierung zurück. Die Standardinstanz ist ein "grün-gelb-rot" 3ColorScale. Gültig nur für type = ColorScale. |
| [GetTop10](./gettop10/) | Gibt die "Top10"-Instanz der bedingten Formatierung zurück. Die Standardregel hebt Zellen hervor, deren Werte in den Top‑10‑Bereich fallen. Gültig nur für type ist Top10. |
| [GetAboveAverage](./getaboveaverage/) | Gibt die "AboveAverage"-Instanz der bedingten Formatierung zurück. Die Standardregel hebt Zellen hervor, die über dem Durchschnitt aller Werte im Bereich liegen. Gültig nur für type = AboveAverage. |
| [GetText](./gettext/) | Der Textwert in einer "text contains"-Bedingten-Formatierungsregel. Gültig nur für type = containsText, notContainsText, beginsWith und endsWith. Der Standardwert ist null. |
| [SetText](./settext/) | Der Textwert in einer "text contains"-Bedingten-Formatierungsregel. Gültig nur für type = containsText, notContainsText, beginsWith und endsWith. Der Standardwert ist null. |
| [GetTimePeriod](./gettimeperiod/) | Der anwendbare Zeitraum in einer "date occurrin"-Bedingten-Formatierungsregel. Gültig nur für type ist timePeriod. Der Standardwert ist TimePeriodType.Today. |
| [SetTimePeriod](./settimeperiod/) | Der anwendbare Zeitraum in einer "date occurrin"-Bedingten-Formatierungsregel. Gültig nur für type ist timePeriod. Der Standardwert ist TimePeriodType.Today. |
