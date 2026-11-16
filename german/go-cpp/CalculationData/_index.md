---
title: "CalculationData Klasse"
linktitle: "CalculationData"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "CalculationData Klasse. Kapselt das Objekt, das calculationdata in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/calculationdata/
---

## CalculationData class

Stellt die erforderlichen Daten beim Berechnen einer Funktion dar, wie Funktionsname, Parameter, usw.

```go

type CalculationData struct  {
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
| [GetCalculatedValue](./getcalculatedvalue/) | Liest oder setzt den berechneten Wert für diese Funktion. |
| [SetCalculatedValue](./setcalculatedvalue/) | Liest oder setzt den berechneten Wert für diese Funktion. |
| [GetWorkbook](./getworkbook/) | Liest das Workbook-Objekt, in dem die Funktion ist. |
| [GetWorksheet](./getworksheet/) | Liest das Worksheet-Objekt, in dem die Funktion ist. |
| [GetCellRow](./getcellrow/) | Liest den Zeilenindex der Zelle, in der die Funktion ist. |
| [GetCellColumn](./getcellcolumn/) | Liest den Spaltenindex der Zelle, in der die Funktion ist. |
| [GetCell](./getcell/) | Liest das Cell-Objekt, in dem die Funktion ist. |
| [GetFunctionName](./getfunctionname/) | Liest den Funktionsnamen, der berechnet werden soll. |
| [GetParamCount](./getparamcount/) | Liest die Anzahl der Parameter |
| [GetParamValue](./getparamvalue/) | Liest das dargestellte Werteobjekt des Parameters an einem angegebenen Index. |
| [GetParamValueInArrayMode](./getparamvalueinarraymode/) | Liest den/die Wert(e) des Parameters an einem angegebenen Index. Wenn der Parameter eine Art Ausdruck ist, der berechnet werden muss, wird er im Array‑Modus berechnet. |
| [GetParamText](./getparamtext/) | Liest den wörtlichen Text des Parameters am angegebenen Index. |
