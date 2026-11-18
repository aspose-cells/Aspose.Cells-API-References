---
title: "Top10-klass"
linktitle: "Top10"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "Top10-klass. Inkapslar objektet som representerar top10 i Go."
type: docs
weight: 200
url: /sv/go-cpp/top10/
---

## Top10 class

Beskriv Top10‑villkorsformateringsregeln. Denna villkorsformateringsregel markerar celler vars värden faller inom de översta N eller nedersta N intervallen, enligt specifikationen.

```go

type Top10 struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewTop10](./newtop10/) | Standardkonstruktor. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [IsPercent](./ispercent/) | Hämta eller ange om en "top/bottom n"-regel är en "top/bottom n procent"-regel. Standardvärdet är falskt. |
| [SetIsPercent](./setispercent/) | Hämta eller ange om en "top/bottom n"-regel är en "top/bottom n procent"-regel. Standardvärdet är falskt. |
| [IsBottom](./isbottom/) | Hämta eller ange om en "top/bottom n"-regel är en "bottom n"-regel. Standardvärdet är falskt. |
| [SetIsBottom](./setisbottom/) | Hämta eller ange om en "top/bottom n"-regel är en "bottom n"-regel. Standardvärdet är falskt. |
| [GetRank](./getrank/) | Hämta eller ange värdet på "n" i en "top/bottom n"-villkorsformateringsregel. Om IsPercent är sant måste värdet ligga mellan 0 och 100. Annars måste det ligga mellan 0 och 1000. Standardvärdet är 10. |
| [SetRank](./setrank/) | Hämta eller ange värdet på "n" i en "top/bottom n"-villkorsformateringsregel. Om IsPercent är sant måste värdet ligga mellan 0 och 100. Annars måste det ligga mellan 0 och 1000. Standardvärdet är 10. |
