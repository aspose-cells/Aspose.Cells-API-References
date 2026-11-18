---
title: "CellValueFormatStrategy-enum"
linktitle: "CellValueFormatStrategy"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "CellValueFormatStrategy-enum. Inkapslar objektet som representerar cellvalueformatstrategy i Go."
type: docs
weight: 200
url: /sv/go-cpp/cellvalueformatstrategy/
---

## CellValueFormatStrategy Enum

Anger hur stil ska tillämpas på cellens värde.

```go

type CellValueFormatStrategy int32


```

## Fält

| Fält | Beskrivning |
| --- | --- |
| [None](./none/) | Inte formaterad. |
| [CellStyle](./cellstyle/) | Endast formaterad med cellens ursprungliga stil. |
| [DisplayStyle](./displaystyle/) | Formaterad med cellens visade stil. |
| [DisplayString](./displaystring/) | Hämtar den visade strängen som visas i MS Excel. Den största skillnaden från <see cref="DisplayStyle"/> är att detta alternativ också beaktar kolumnbreddens effekt. Om kolumnbredden är för liten för att visa den formaterade strängen helt, kan "#" visas, precis som MS Excel gör. |
