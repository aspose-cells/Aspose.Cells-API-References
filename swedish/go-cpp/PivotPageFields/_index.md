---
title: "PivotPageFields-klass"
linktitle: "PivotPageFields"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "PivotPageFields-klass. Inkapslar objektet som representerar pivotpagefields i Go."
type: docs
weight: 200
url: /sv/go-cpp/pivotpagefields/
---

## PivotPageFields class

Representerar pivot‑sidobjektenif pivottabellens datakälla är konsolideringsområden. Det kan bara innehålla upp till 4 objekt.

```go

type PivotPageFields struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewPivotPageFields](./newpivotpagefields/) | Representerar pivot‑sidfältsposterna. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [AddPageField](./addpagefield/) | Lägger till ett sidfält. |
| [GetPageFieldCount](./getpagefieldcount/) | Hämtar antalet sidfält. |
| [AddIdentify](./addidentify/) | Ställer in vilken objektetikett i varje sidfält som ska användas för att identifiera dataområdet. pageItemIndex.Length måste vara lika med PageFieldCount, så lägg till sidfältet först. |
