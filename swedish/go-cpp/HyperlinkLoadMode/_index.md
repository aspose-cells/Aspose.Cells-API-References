---
title: "HyperlinkLoadMode-enum"
linktitle: "HyperlinkLoadMode"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "HyperlinkLoadMode-enum. Inkapslar objektet som representerar hyperlinkloadmode i Go."
type: docs
weight: 200
url: /sv/go-cpp/hyperlinkloadmode/
---

## HyperlinkLoadMode Enum

Anger hur hyperlänkar hanteras när HTML laddas.

```go

type HyperlinkLoadMode int32


```

## Fält

| Fält | Beskrivning |
| --- | --- |
| [Normal](./normal/) | Endast den första hyperlänken i en cell laddas, efterföljande ignoreras. |
| [AllowMultiple](./allowmultiple/) | Alla hyperlänkar i en cell läggs till i <see cref="Worksheet.Hyperlinks"/>. Observera att MS Excel endast stöder en hyperlänk per cell, så detta alternativ kan producera filer som Excel inte kan rendera fullt ut. |
