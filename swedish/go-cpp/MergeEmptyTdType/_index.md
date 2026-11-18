---
title: "MergeEmptyTdType enum"
linktitle: "MergeEmptyTdType"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "MergeEmptyTdType‑enum. Inkapslar objektet som representerar mergeemptytdtype i Go."
type: docs
weight: 200
url: /sv/go-cpp/mergeemptytdtype/
---

## MergeEmptyTdType Enum

Representerar sammanslagningstypen för ett tomt TD-element när en fil exporteras till HTML.

```go

type MergeEmptyTdType int32


```

## Fält

| Fält | Beskrivning |
| --- | --- |
| [Default](./default/) | Visning som MS Excel. |
| [None](./none/) | Tomma TD‑element kommer inte att slås ihop vid export av fil till html. Detta kommer att generera en avsevärt större html‑fil. |
| [MergeForcely](./mergeforcely/) | Tvingad sammanslagning av tomma TD‑element vid export av fil till html. Storleken på html‑filen kommer att minskas avsevärt efter att värdet satts till true. Om du vill importera html‑filen till Excel eller exportera perfekta rutnätslinjer när du sparar filen till html, behåll standardvärdet. |
