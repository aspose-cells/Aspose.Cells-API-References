---
title: "FindOptions Class"
linktitle: "FindOptions"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "FindOptions class. Inkapslar objektet som representerar findoptions i Go."
type: docs
weight: 200
url: /sv/go-cpp/findoptions/
---

## FindOptions class

Representerar sökalternativ.

```go

type FindOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewFindOptions](./newfindoptions/) | Standardkonstruktor. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetCaseSensitive](./getcasesensitive/) | Indikerar om den sökta strängen är skiftlägeskänslig. |
| [SetCaseSensitive](./setcasesensitive/) | Indikerar om den sökta strängen är skiftlägeskänslig. |
| [GetLookAtType](./getlookattype/) | Titta på typ. |
| [SetLookAtType](./setlookattype/) | Titta på typ. |
| [GetRange](./getrange/) | Hämtar och anger det sökta intervallet. |
| [SetRange](./setrange/) | Anger det sökta intervallet. |
| [IsRangeSet](./israngeset/) | Anger om det sökta intervallet är angivet. |
| [GetSearchBackward](./getsearchbackward/) | Om sökningen ska gå bakåt för celler. |
| [SetSearchBackward](./setsearchbackward/) | Om sökningen ska gå bakåt för celler. |
| [GetSearchOrderByRows](./getsearchorderbyrows/) | Anger om sökordningen är per rader eller kolumner. |
| [SetSearchOrderByRows](./setsearchorderbyrows/) | Anger om sökordningen är per rader eller kolumner. |
| [GetLookInType](./getlookintype/) | Sök i typ. |
| [SetLookInType](./setlookintype/) | Sök i typ. |
| [GetRegexKey](./getregexkey/) | Anger om den sökta nyckeln är ett regex. Om true tas den sökta nyckeln som regex och tolkas. Annars tolkas nyckeln enligt reglerna i MS Excel. |
| [SetRegexKey](./setregexkey/) | Anger om den sökta nyckeln är ett regex. Om true tas den sökta nyckeln som regex och tolkas. Annars tolkas nyckeln enligt reglerna i MS Excel. |
| [GetValueTypeSensitive](./getvaluetypesensitive/) | Anger om den sökta cellvärdestypen ska vara samma som den sökta nyckeln. |
| [SetValueTypeSensitive](./setvaluetypesensitive/) | Anger om den sökta cellvärdestypen ska vara samma som den sökta nyckeln. |
| [GetStyle](./getstyle/) | Formatet att söka efter. |
| [SetStyle](./setstyle/) | Formatet att söka efter. |
| [GetConvertNumericData](./getconvertnumericdata/) | Hämtar eller anger ett värde som anger om den sökta strängvärdet ska konverteras till numerisk data. |
| [SetConvertNumericData](./setconvertnumericdata/) | Hämtar eller anger ett värde som anger om den sökta strängvärdet ska konverteras till numerisk data. |
