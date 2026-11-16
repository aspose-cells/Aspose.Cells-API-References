---
title: "SplitPartInfo Classe"
linktitle: "SplitPartInfo"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe SplitPartInfo. Encapsule l'objet qui représente splitpartinfo en Go."
type: docs
weight: 200
url: /fr/go-cpp/splitpartinfo/
---

## SplitPartInfo class

Représente les informations d'une entrée/sortie pour plusieurs entrées/sorties, comme la page actuelle à rendre lors de la conversion d'une feuille de calcul en image.

```go

type SplitPartInfo struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetPartIndex](./getpartindex/) | Indice de la partie actuelle dans la séquence (base 0). -1 signifie qu'il n'y a pas de parties multiples, donc le résultat est unique. |
| [GetSheetIndex](./getsheetindex/) | Indice de la feuille où se trouve la partie actuelle. -1 indique qu'il n'y a qu'une seule feuille. |
| [GetSheetName](./getsheetname/) | Nom de la feuille où se trouve la partie actuelle. |
