---
title: "RowCollection klass"
linktitle: "RowCollection"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "RowCollection-klass. Inkapslar objektet som representerar rowcollection i Go."
type: docs
weight: 200
url: /sv/go-cpp/rowcollection/
---

## RowCollection class

Samlar <see cref=\"Row\"/>-objekten som representerar de enskilda raderna i ett arbetsblad.

```go

type RowCollection struct  {
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
| [GetCount](./getcount/) | Hämtar antalet rader i denna samling. |
| [GetEnumerator](./getenumerator/) | Hämtar en enumerator som itererar rader genom denna samling |
| [GetEnumerator_Bool_Bool](./getenumerator_bool_bool/) | Hämtar en enumerator som itererar rader genom denna samling |
| [GetRowByIndex](./getrowbyindex/) | Hämtar radobjektet efter positionen i listan. |
| [Get](./get/) | Hämtar ett Row‑objekt med angivet radindex. Row‑objektet för det angivna radindexet kommer att instansieras om det inte redan finns. |
| [Clear](./clear/) | Rensa alla rader och celler. |
| [RemoveAt](./removeat/) | Ta bort radobjektet på det angivna indexet (positionen) i denna samling. |
