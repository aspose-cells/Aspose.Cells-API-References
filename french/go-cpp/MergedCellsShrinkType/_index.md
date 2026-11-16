---
title: "Enum MergedCellsShrinkType"
linktitle: "MergedCellsShrinkType"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Enum MergedCellsShrinkType. Encapsule l'objet qui représente mergedcellsshrinktype en Go."
type: docs
weight: 200
url: /fr/go-cpp/mergedcellsshrinktype/
---

## MergedCellsShrinkType Enum

Représente la stratégie de réduction des cellules fusionnées pour des opérations telles que la suppression de lignes/colonnes vides.

```go

type MergedCellsShrinkType int32


```

## Champs

| Champ | Description |
| --- | --- |
| [None](./none/) | Laisse les cellules fusionnées telles quelles, sans aucune modification. |
| [ShrinkToFit](./shrinktofit/) | Réduit la zone fusionnée si nécessaire, en supprimant les lignes du bas ou les colonnes de droite, tout en veillant à ce que tout le contenu reste visible. |
| [KeepHeaderOnly](./keepheaderonly/) | Ne conserve que les lignes/colonnes d'en-tête de la zone fusionnée lorsque la cellule supérieure gauche de la zone fusionnée n'est pas vide. |
