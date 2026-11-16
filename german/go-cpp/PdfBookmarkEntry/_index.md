---
title: "PdfBookmarkEntry Klasse"
linktitle: "PdfBookmarkEntry"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "PdfBookmarkEntry Klasse. Kapselt das Objekt, das pdfbookmarkentry in Go repräsentiert."
type: docs
weight: 200
url: /de/go-cpp/pdfbookmarkentry/
---

## PdfBookmarkEntry class

PdfBookmarkEntry ist ein Eintrag im PDF-Lesezeichen. Wenn die Text-Eigenschaft der aktuellen Instanz null oder "" ist, wird die aktuelle Instanz ausgeblendet und die Kinder werden auf derselben Ebene eingefügt.

```go

type PdfBookmarkEntry struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewPdfBookmarkEntry](./newpdfbookmarkentry/) | Standardkonstruktor. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetText](./gettext/) | Titel eines Lesezeichens. |
| [SetText](./settext/) | Titel eines Lesezeichens. |
| [GetDestination](./getdestination/) | Die Zelle, zu der der Lesezeichen-Link führt. |
| [SetDestination](./setdestination/) | Die Zelle, zu der der Lesezeichen-Link führt. |
| [GetDestinationName](./getdestinationname/) | Liest oder setzt den Namen des Ziels. |
| [SetDestinationName](./setdestinationname/) | Liest oder setzt den Namen des Ziels. |
| [IsOpen](./isopen/) | Wenn diese Eigenschaft wahr ist, wird der Lesezeichen-Eintrag erweitert, andernfalls wird er zusammengeklappt. |
| [SetIsOpen](./setisopen/) | Wenn diese Eigenschaft wahr ist, wird der Lesezeichen-Eintrag erweitert, andernfalls wird er zusammengeklappt. |
| [IsCollapse](./iscollapse/) | Wenn diese Eigenschaft wahr ist, wird der Lesezeichen-Eintrag zusammengeklappt, andernfalls wird er erweitert. |
| [SetIsCollapse](./setiscollapse/) | Wenn diese Eigenschaft wahr ist, wird der Lesezeichen-Eintrag zusammengeklappt, andernfalls wird er erweitert. |
