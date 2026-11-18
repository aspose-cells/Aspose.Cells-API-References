---
title: "PdfBookmarkEntry Klass"
linktitle: "PdfBookmarkEntry"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "PdfBookmarkEntry klass. Inkapslar objektet som representerar pdfbookmarkentry i Go."
type: docs
weight: 200
url: /sv/go-cpp/pdfbookmarkentry/
---

## PdfBookmarkEntry class

PdfBookmarkEntry är ett objekt i PDF-bokmärken. Om Text‑egenskapen för den aktuella instansen är null eller \"\", kommer den aktuella instansen att döljas och barnobjekt kommer att infogas på samma nivå.

```go

type PdfBookmarkEntry struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewPdfBookmarkEntry](./newpdfbookmarkentry/) | Standardkonstruktor. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetText](./gettext/) | Titel på ett bokmärke. |
| [SetText](./settext/) | Titel på ett bokmärke. |
| [GetDestination](./getdestination/) | Cellen som bokmärkeslänken pekar på. |
| [SetDestination](./setdestination/) | Cellen som bokmärkeslänken pekar på. |
| [GetDestinationName](./getdestinationname/) | Hämtar eller anger namn på destinationen. |
| [SetDestinationName](./setdestinationname/) | Hämtar eller anger namn på destinationen. |
| [IsOpen](./isopen/) | När detta egenskap är sann, kommer bookmarkentry att expandera, annars kommer den att kollapsa. |
| [SetIsOpen](./setisopen/) | När detta egenskap är sann, kommer bookmarkentry att expandera, annars kommer den att kollapsa. |
| [IsCollapse](./iscollapse/) | När detta egenskap är sann, kommer bookmarkentry att kollapsa, annars kommer den att expandera. |
| [SetIsCollapse](./setiscollapse/) | När detta egenskap är sann, kommer bookmarkentry att kollapsa, annars kommer den att expandera. |
