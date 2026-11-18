---
title: "AbstractLowCodeLoadOptionsProvider-klass"
linktitle: "AbstractLowCodeLoadOptionsProvider"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "AbstractLowCodeLoadOptionsProvider-klass. Inkapslar objektet som representerar abstractlowcodeloadoptionsprovider i Go."
type: docs
weight: 200
url: /sv/go-cpp/abstractlowcodeloadoptionsprovider/
---

## AbstractLowCodeLoadOptionsProvider class

Implementering för att tillhandahålla flera inläsningsalternativ för processer som använder flera indata (t.ex. mallfiler).

```go

type AbstractLowCodeLoadOptionsProvider struct  {
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
| [MoveNext](./movenext/) | Kontrollerar om det finns mer indata. |
| [GetCurrent](./getcurrent/) | Hämtar laddningsalternativen från vilka data för den för närvarande bearbetade delen ska läsas in. |
| [Finish](./finish/) | Frigör resurser efter att ha bearbetat den aktuella delen av indata. |
