---
title: "CalculationData klass"
linktitle: "CalculationData"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "CalculationData klass. Inkapslar objektet som representerar calculationdata i Go."
type: docs
weight: 200
url: /sv/go-cpp/calculationdata/
---

## CalculationData class

Representerar den nödvändiga datan vid beräkning av en funktion, såsom funktionsnamn, parametrar, med mera.

```go

type CalculationData struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetCalculatedValue](./getcalculatedvalue/) | Hämtar eller anger det beräknade värdet för denna funktion. |
| [SetCalculatedValue](./setcalculatedvalue/) | Hämtar eller anger det beräknade värdet för denna funktion. |
| [GetWorkbook](./getworkbook/) | Hämtar Workbook-objektet där funktionen är. |
| [GetWorksheet](./getworksheet/) | Hämtar Worksheet-objektet där funktionen är. |
| [GetCellRow](./getcellrow/) | Hämtar radindexet för cellen där funktionen är. |
| [GetCellColumn](./getcellcolumn/) | Hämtar kolumnindexet för cellen där funktionen är. |
| [GetCell](./getcell/) | Hämtar Cell-objektet där funktionen är. |
| [GetFunctionName](./getfunctionname/) | Hämtar funktionsnamnet som ska beräknas. |
| [GetParamCount](./getparamcount/) | Hämtar antalet parametrar |
| [GetParamValue](./getparamvalue/) | Hämtar det representerade värdeobjektet för parametern på ett givet index. |
| [GetParamValueInArrayMode](./getparamvalueinarraymode/) | Hämtar värdet/värdena för parametern på ett givet index. Om parametern är någon form av uttryck som måste beräknas, beräknas den i arrayläge. |
| [GetParamText](./getparamtext/) | Hämtar den bokstavliga texten för parametern på det givna indexet. |
