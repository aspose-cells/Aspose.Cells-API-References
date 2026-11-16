---
title: "Classe PivotPageFields"
linktitle: "PivotPageFields"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "PivotPageFields class. Encapsule l'objet qui représente pivotpagefields en Go."
type: docs
weight: 200
url: /fr/go-cpp/pivotpagefields/
---

## PivotPageFields class

Représente les éléments de page du tableau croisé dynamique si la source de données du tableau croisé dynamique est des plages de consolidation. Il ne peut contenir que jusqu'à 4 éléments.

```go

type PivotPageFields struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewPivotPageFields](./newpivotpagefields/) | Représente les éléments de champ de page pivot. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [AddPageField](./addpagefield/) | Ajoute un champ de page. |
| [GetPageFieldCount](./getpagefieldcount/) | Obtient le nombre de champs de page. |
| [AddIdentify](./addidentify/) | Définit quelle étiquette d'élément dans chaque champ de page utiliser pour identifier la plage de données. La pageItemIndex.Length doit être égale à PageFieldCount, veuillez donc ajouter d'abord le champ de page. |
