---
title: "CopyOptions klass"
linktitle: "CopyOptions"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "CopyOptions klass. Inkapslar objektet som representerar copyoptions i Go."
type: docs
weight: 200
url: /sv/go-cpp/copyoptions/
---

## CopyOptions class

Representerar kopieringsalternativen.

```go

type CopyOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewCopyOptions](./newcopyoptions/) | CopyOptions-konstruktor. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetKeepMacros](./getkeepmacros/) | Anger om makron ska behållas; |
| [SetKeepMacros](./setkeepmacros/) | Anger om makron ska behållas; |
| [GetExtendToAdjacentRange](./getextendtoadjacentrange/) | Anger om intervall ska utökas när intervallet kopieras till intilliggande intervall. |
| [SetExtendToAdjacentRange](./setextendtoadjacentrange/) | Anger om intervall ska utökas när intervallet kopieras till intilliggande intervall. |
| [GetCopyNames](./getcopynames/) | Anger om namnen ska kopieras. |
| [SetCopyNames](./setcopynames/) | Anger om namnen ska kopieras. |
| [GetCopyInvalidFormulasAsValues](./getcopyinvalidformulasasvalues/) | Om formeln inte är giltig för destinationsmålet, kopieras endast värden. |
| [SetCopyInvalidFormulasAsValues](./setcopyinvalidformulasasvalues/) | Om formeln inte är giltig för destinationsmålet, kopieras endast värden. |
| [GetColumnCharacterWidth](./getcolumncharacterwidth/) | Anger om kolumnbredd ska kopieras i teckenenheter. |
| [SetColumnCharacterWidth](./setcolumncharacterwidth/) | Anger om kolumnbredd ska kopieras i teckenenheter. |
| [GetReferToSheetWithSameName](./getrefertosheetwithsamename/) | I ms excel, när du kopierar formler som refererar till andra kalkylblad medan du kopierar ett kalkylblad till ett annat, ska de kopierade formlerna referera till källarboken. Men i vissa situationer kan användaren behöva att de kopierade formlerna refererar till kalkylblad med samma namn i samma arbetsbok, till exempel när dessa kalkylblad redan har kopierats innan denna kopieringsåtgärd, då bör denna egenskap hållas som true. |
| [SetReferToSheetWithSameName](./setrefertosheetwithsamename/) | I ms excel, när du kopierar formler som refererar till andra kalkylblad medan du kopierar ett kalkylblad till ett annat, ska de kopierade formlerna referera till källarboken. Men i vissa situationer kan användaren behöva att de kopierade formlerna refererar till kalkylblad med samma namn i samma arbetsbok, till exempel när dessa kalkylblad redan har kopierats innan denna kopieringsåtgärd, då bör denna egenskap hållas som true. |
| [GetReferToDestinationSheet](./getrefertodestinationsheet/) | När du kopierar intervallet i samma fil och diagrammet refererar till källbladet, betyder False att den kopierade diagrammets datakälla inte kommer att ändras. True betyder att den kopierade diagrammets datakälla refererar till destinationsbladet. |
| [SetReferToDestinationSheet](./setrefertodestinationsheet/) | När du kopierar intervallet i samma fil och diagrammet refererar till källbladet, betyder False att den kopierade diagrammets datakälla inte kommer att ändras. True betyder att den kopierade diagrammets datakälla refererar till destinationsbladet. |
| [GetUpdateInvalidReferencesToTargetSheet](./getupdateinvalidreferencestotargetsheet/) | Anger om man ska referera till målarkbladet om det refererade kalkylbladet inte har kopierats. |
| [SetUpdateInvalidReferencesToTargetSheet](./setupdateinvalidreferencestotargetsheet/) | Anger om man ska referera till målarkbladet om det refererade kalkylbladet inte har kopierats. |
