---
title: "MergeEmptyTdType Enum"
linktitle: "MergeEmptyTdType"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Enum MergeEmptyTdType. Encapsule l’objet qui représente mergeemptytdtype en Go."
type: docs
weight: 200
url: /fr/go-cpp/mergeemptytdtype/
---

## MergeEmptyTdType Enum

Représente le type de fusion pour un élément TD vide lors de l'exportation d'un fichier en HTML.

```go

type MergeEmptyTdType int32


```

## Champs

| Champ | Description |
| --- | --- |
| [Default](./default/) | Affichage similaire à MS Excel. |
| [None](./none/) | Les éléments TD vides ne seront pas fusionnés lors de l’exportation du fichier en HTML. Cela générera un fichier HTML nettement plus volumineux. |
| [MergeForcely](./mergeforcely/) | Fusion forcée des éléments TD vides lors de l’exportation du fichier en HTML. La taille du fichier HTML sera considérablement réduite après avoir défini la valeur sur true. Si vous souhaitez importer le fichier HTML dans Excel ou exporter des lignes de grille parfaites lors de l’enregistrement du fichier en HTML, veuillez conserver la valeur par défaut. |
