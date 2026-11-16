---
title: "PdfBookmarkEntry Classe"
linktitle: "PdfBookmarkEntry"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "PdfBookmarkEntry classe. Encapsule l'objet qui représente pdfbookmarkentry en Go."
type: docs
weight: 200
url: /fr/go-cpp/pdfbookmarkentry/
---

## PdfBookmarkEntry class

PdfBookmarkEntry est une entrée dans le signet pdf. Si la propriété Text de l'instance actuelle est null ou \"\", l'instance actuelle sera masquée et les enfants seront insérés au même niveau.

```go

type PdfBookmarkEntry struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewPdfBookmarkEntry](./newpdfbookmarkentry/) | Constructeur par défaut. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetText](./gettext/) | Titre d'un signet. |
| [SetText](./settext/) | Titre d'un signet. |
| [GetDestination](./getdestination/) | La cellule vers laquelle le lien du signet. |
| [SetDestination](./setdestination/) | La cellule vers laquelle le lien du signet. |
| [GetDestinationName](./getdestinationname/) | Obtient ou définit le nom de la destination. |
| [SetDestinationName](./setdestinationname/) | Obtient ou définit le nom de la destination. |
| [IsOpen](./isopen/) | Lorsque cette propriété est vraie, le bookmarkentry s'étendra, sinon il se repliera. |
| [SetIsOpen](./setisopen/) | Lorsque cette propriété est vraie, le bookmarkentry s'étendra, sinon il se repliera. |
| [IsCollapse](./iscollapse/) | Lorsque cette propriété est vraie, le bookmarkentry se repliera, sinon il s'étendra. |
| [SetIsCollapse](./setiscollapse/) | Lorsque cette propriété est vraie, le bookmarkentry se repliera, sinon il s'étendra. |
