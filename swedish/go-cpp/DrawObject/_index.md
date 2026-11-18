---
title: "DrawObject-klass"
linktitle: "DrawObject"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "DrawObject-klass. Inkapslar objektet som representerar drawobject i Go."
type: docs
weight: 200
url: /sv/go-cpp/drawobject/
---

## DrawObject class

DrawObject kommer att initieras och returneras vid rendering.

```go

type DrawObject struct  {
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
| [GetCell](./getcell/) | Anger Cell-objektet vid rendering. Alla egenskaper för cellen kan nås. |
| [GetShape](./getshape/) | Anger Shape-objektet vid rendering. Alla egenskaper för shape kan nås. |
| [GetImageBytes](./getimagebytes/) | Anger bildbytes för renderad Chart, Shape vid rendering. |
| [GetType](./gettype/) | Anger typen av DrawObject. |
| [GetCurrentPage](./getcurrentpage/) | Anger sidindex för DrawObject. Sidindex är nollbaserad. Ett blad innehåller flera sidor vid rendering. |
| [GetTotalPages](./gettotalpages/) | Anger totalt antal sidor i aktuell rendering. |
| [GetSheetIndex](./getsheetindex/) | Anger aktuellt bladindex för DrawObject. |
