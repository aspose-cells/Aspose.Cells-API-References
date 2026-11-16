---
title: "Classe RevisionCellComment"
linktitle: "RevisionCellComment"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe RevisionCellComment. Encapsule l'objet qui représente le commentaire de révision dans Go."
type: docs
weight: 200
url: /fr/go-cpp/revisioncellcomment/
---

## RevisionCellComment class

Représente un enregistrement de révision d'une modification de commentaire de cellule.

```go

type RevisionCellComment struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewRevisionCellComment](./newrevisioncellcomment/) | Construit à partir d'un objet parent. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetType](./gettype/) | Obtient le type de révision. |
| [GetRow](./getrow/) | Obtient l'index de ligne de l'élément qui contient un commentaire. |
| [GetColumn](./getcolumn/) | Obtient l'index de colonne de l'élément qui contient un commentaire. |
| [GetCellName](./getcellname/) | Obtient le nom de la cellule. |
| [SetCellName](./setcellname/) | Obtient le nom de la cellule. |
| [GetActionType](./getactiontype/) | Obtient le type d'action de la révision. |
| [IsOldComment](./isoldcomment/) | Indique s'il s'agit d'un ancien commentaire. |
| [GetOldLength](./getoldlength/) | Obtient la longueur du texte du commentaire ajouté dans cette révision. |
| [GetNewLength](./getnewlength/) | Obtient la longueur du commentaire avant que cette révision ne soit effectuée. |
| [GetWorksheet](./getworksheet/) | Obtient la feuille de calcul. |
| [GetId](./getid/) | Obtient le numéro de cette révision. |
