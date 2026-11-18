---
title: "HtmlCrossType Enum"
linktitle: "HtmlCrossType"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "HtmlCrossType enum. Inkapslar objektet som representerar htmlcrosstype i Go."
type: docs
weight: 200
url: /sv/go-cpp/htmlcrosstype/
---

## HtmlCrossType Enum

Representerar fem typer av HTML-korssträng.

```go

type HtmlCrossType int32


```

## Fält

| Fält | Beskrivning |
| --- | --- |
| [Default](./default/) | Visas som i MS Excel, beror på nästa cell. Om nästa cell är null, kommer strängen att korsas, eller så trunkeras den. |
| [MSExport](./msexport/) | Visar strängen som i MS Excel vid export av html. |
| [Cross](./cross/) | Visar HTML-korssträng, denna prestanda för att skapa stora html-filer blir mer än tio gånger snabbare än att sätta värdet till Default eller FitToCell. |
| [CrossHideRight](./crosshideright/) | Visar HTML-korssträng och döljer den högra strängen när texterna överlappar. |
| [FitToCell](./fittocell/) | Visar endast strängen inom cellens bredd. |
