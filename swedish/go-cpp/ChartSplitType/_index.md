---
title: "ChartSplitType-enum"
linktitle: "ChartSplitType"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "ChartSplitType-enum. Inkapslar objektet som representerar chartsplittype i Go."
type: docs
weight: 200
url: /sv/go-cpp/chartsplittype/
---

## ChartSplitType Enum

Representerar hur de två sektionerna i antingen ett paj-i-paj-diagram eller ett stapel-i-paj-diagram delas.

```go

type ChartSplitType int32


```

## Fält

| Fält | Beskrivning |
| --- | --- |
| [Position](./position/) | Representerar datapunkterna. Datapunkterna ska delas mellan pajdiagrammet och det andra diagrammet genom att placera den sista delningspositionen för datapunkterna i det andra diagrammet. |
| [Value](./value/) | Representerar datapunkterna som ska delas mellan pajdiagrammet och det andra diagrammet genom att placera datapunkterna med värde mindre än Split Position i det andra diagrammet. |
| [PercentValue](./percentvalue/) | Representerar datapunkterna som ska delas mellan pajdiagrammet och det andra diagrammet genom att placera punkterna med en procentandel mindre än Split Position-procenten i det andra diagrammet. |
| [Custom](./custom/) | Representerar datapunkterna som ska delas mellan pajdiagrammet och det andra diagrammet enligt de anpassade delningsvärdena. |
| [Auto](./auto/) | Representerar datapunkterna som ska delas med standardmekanismen för den här diagramtypen. |
