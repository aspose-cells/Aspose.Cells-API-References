---
title: "PdfBookmarkEntry Classe"
linktitle: "PdfBookmarkEntry"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "PdfBookmarkEntry class. Incapsula l'oggetto che rappresenta pdfbookmarkentry in Go."
type: docs
weight: 200
url: /it/go-cpp/pdfbookmarkentry/
---

## PdfBookmarkEntry class

PdfBookmarkEntry è una voce nel segnalibro PDF. Se la proprietà Text dell'istanza corrente è null o "", l'istanza corrente sarà nascosta e i figli saranno inseriti al livello corrente.

```go

type PdfBookmarkEntry struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewPdfBookmarkEntry](./newpdfbookmarkentry/) | Costruttore predefinito. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetText](./gettext/) | Titolo di un segnalibro. |
| [SetText](./settext/) | Titolo di un segnalibro. |
| [GetDestination](./getdestination/) | La cella a cui punta il collegamento del segnalibro. |
| [SetDestination](./setdestination/) | La cella a cui punta il collegamento del segnalibro. |
| [GetDestinationName](./getdestinationname/) | Ottiene o imposta il nome della destinazione. |
| [SetDestinationName](./setdestinationname/) | Ottiene o imposta il nome della destinazione. |
| [IsOpen](./isopen/) | Quando questa proprietà è vera, la voce del segnalibro si espanderà, altrimenti si chiuderà. |
| [SetIsOpen](./setisopen/) | Quando questa proprietà è vera, la voce del segnalibro si espanderà, altrimenti si chiuderà. |
| [IsCollapse](./iscollapse/) | Quando questa proprietà è vera, la voce del segnalibro si chiuderà, altrimenti si espanderà. |
| [SetIsCollapse](./setiscollapse/) | Quando questa proprietà è vera, la voce del segnalibro si chiuderà, altrimenti si espanderà. |
