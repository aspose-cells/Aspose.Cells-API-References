---
title: "PdfBookmarkEntry Clase"
linktitle: "PdfBookmarkEntry"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "PdfBookmarkEntry clase. Encapsula el objeto que representa pdfbookmarkentry en Go."
type: docs
weight: 200
url: /es/go-cpp/pdfbookmarkentry/
---

## PdfBookmarkEntry class

PdfBookmarkEntry is an entry in pdf bookmark.if Text property of current instance is null or "",current instance will be hidden and children will be inserted on current level.

```go

type PdfBookmarkEntry struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
| [NewPdfBookmarkEntry](./newpdfbookmarkentry/) | Default constructor. |

## Methods

| Method | Description |
| --- | --- |
| [IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
| [GetText](./gettext/) | Título de un marcador. |
| [SetText](./settext/) | Título de un marcador. |
| [GetDestination](./getdestination/) | La celda a la que apunta el enlace del marcador. |
| [SetDestination](./setdestination/) | La celda a la que apunta el enlace del marcador. |
| [GetDestinationName](./getdestinationname/) | Obtiene o establece el nombre del destino. |
| [SetDestinationName](./setdestinationname/) | Obtiene o establece el nombre del destino. |
| [IsOpen](./isopen/) | Cuando esta propiedad es verdadera, la entrada del marcador se expandirá; de lo contrario, se contraerá. |
| [SetIsOpen](./setisopen/) | Cuando esta propiedad es verdadera, la entrada del marcador se expandirá; de lo contrario, se contraerá. |
| [IsCollapse](./iscollapse/) | Cuando esta propiedad es verdadera, la entrada del marcador se contraerá; de lo contrario, se expandirá. |
| [SetIsCollapse](./setiscollapse/) | Cuando esta propiedad es verdadera, la entrada del marcador se contraerá; de lo contrario, se expandirá. |
