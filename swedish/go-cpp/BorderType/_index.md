---
title: "BorderType-enum"
linktitle: "BorderType"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "BorderType-enum. Inkapslar objektet som representerar bordertype i Go."
type: docs
weight: 200
url: /sv/go-cpp/bordertype/
---

## BorderType Enum

Enumererar typer av kantlinjer och diagonala linjer.

```go

type BorderType int32


```

## Fält

| Fält | Beskrivning |
| --- | --- |
| [LeftBorder](./leftborder/) | Representerar vänster kantlinje. |
| [RightBorder](./rightborder/) | Representerar att högra kantlinjen finns. |
| [TopBorder](./topborder/) | Representerar den övre kantlinjen. |
| [BottomBorder](./bottomborder/) | Representerar den nedre kantlinjen. |
| [DiagonalDown](./diagonaldown/) | Representerar den diagonala linjen från övre vänster till nedre höger. |
| [DiagonalUp](./diagonalup/) | Representerar den diagonala linjen från nedre vänster till övre höger. |
| [Vertical](./vertical/) | Endast för dynamisk stil, såsom villkorsstyrd formatering, pivottabell. |
| [Horizontal](./horizontal/) | Endast för dynamisk stil, såsom villkorsstyrd formatering, pivottabell. |
| [SideBorders](./sideborders/) | Anger de fyra sidokanterna: <see cref="LeftBorder"/>,<see cref="RightBorder"/>, <see cref="TopBorder"/> och <see cref="BottomBorder"/>. |
| [Diagonal](./diagonal/) | Special kombination av flera kanter för användarens bekvämlighet för vissa API:er.Anger diagonala kanter av <see cref="DiagonalUp"/> och <see cref="DiagonalDown"/>. |
| [DynamicStyleBorders](./dynamicstyleborders/) | Anger <see cref="Vertical"/> och <see cref="Horizontal"/> för dynamisk stil. |
| [None](./none/) | Ingen kant har specificerats. |
