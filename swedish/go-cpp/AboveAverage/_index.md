---
title: "AboveAverage klass"
linktitle: "AboveAverage"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "AboveAverage klass. Inkapslar objektet som representerar aboveaverage i Go."
type: docs
weight: 200
url: /sv/go-cpp/aboveaverage/
---

## AboveAverage class

Beskriv regeln för villkorsstyrd formatering AboveAverage. Denna villkorsstyrda formateringsregel markerar celler som är över eller under genomsnittet för alla värden i intervallet.

```go

type AboveAverage struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewAboveAverage](./newaboveaverage/) | Standardkonstruktor. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [IsAboveAverage](./isaboveaverage/) | Hämta eller ange flaggan som indikerar om regeln är en \"above average\"-regel.'true' indikerar 'above average'.Standardvärdet är true. |
| [SetIsAboveAverage](./setisaboveaverage/) | Hämta eller ange flaggan som indikerar om regeln är en \"above average\"-regel.'true' indikerar 'above average'.Standardvärdet är true. |
| [IsEqualAverage](./isequalaverage/) | Hämta eller ange flaggan som indikerar om kriterierna 'aboveAverage' och 'belowAverage' är inklusiva för själva medelvärdet, eller exkluderar det värdet.'true' indikerar att medelvärdet inkluderas i kriterierna.Standardvärdet är false. |
| [SetIsEqualAverage](./setisequalaverage/) | Hämta eller ange flaggan som indikerar om kriterierna 'aboveAverage' och 'belowAverage' är inklusiva för själva medelvärdet, eller exkluderar det värdet.'true' indikerar att medelvärdet inkluderas i kriterierna.Standardvärdet är false. |
| [GetStdDev](./getstddev/) | Hämta eller ange antalet standardavvikelser som ska inkluderas över eller under medelvärdet i det villkorsformatregeln.Inmatningsvärdet måste vara mellan 0 och 3 (inkludera 0 och 3).Att sätta detta värde till 0 betyder att stdDev inte är angivet.Standardvärdet är 0. |
| [SetStdDev](./setstddev/) | Hämta eller ange antalet standardavvikelser som ska inkluderas över eller under medelvärdet i det villkorsformatregeln.Inmatningsvärdet måste vara mellan 0 och 3 (inkludera 0 och 3).Att sätta detta värde till 0 betyder att stdDev inte är angivet.Standardvärdet är 0. |
