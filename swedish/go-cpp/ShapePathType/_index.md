---
title: "ShapePathType Enum"
linktitle: "ShapePathType"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "ShapePathType enum. Inkapslar objektet som representerar shapepathtype i Go."
type: docs
weight: 200
url: /sv/go-cpp/shapepathtype/
---

## ShapePathType Enum

Representerar segmenttypen för sökväg.

```go

type ShapePathType int32


```

## Fält

| Fält | Beskrivning |
| --- | --- |
| [LineTo](./lineto/) | Rakt linjesegment |
| [CubicBezierCurveTo](./cubicbeziercurveto/) | Kubisk Bézier-kurva |
| [MoveTo](./moveto/) | Starta en ny bana |
| [Close](./close/) | Om start‑POINT och slut‑POINT inte är desamma, ritas en enkel rak linje för att koppla ihop start‑POINT och slut‑POINT för banan. |
| [End](./end/) | Slutet på den aktuella banan |
| [Escape](./escape/) | Escape |
| [ArcTo](./arcto/) | En båge |
| [Unknown](./unknown/) | Okänd |
