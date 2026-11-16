---
title: "Enum AccessCacheOptions"
linktitle: "AccessCacheOptions"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Enum AccessCacheOptions. Encapsule l'objet qui représente accesscacheoptions en Go."
type: docs
weight: 200
url: /fr/go-cpp/accesscacheoptions/
---

## AccessCacheOptions Enum

Options de mise en cache pour l'accès aux données. Plusieurs options peuvent être combinées en utilisant l'opérateur "|".

```go

type AccessCacheOptions int32


```

## Champs

| Champ | Description |
| --- | --- |
| [None](./none/) | Pas de cache pour aucun accès aux données. |
| [All](./all/) | Appliquer toutes les optimisations possibles pour tous les types d'accès aux données dans le classeur. Tous les paramètres et données ne doivent pas être modifiés pendant l'accès optimisé. |
| [PositionAndSize](./positionandsize/) | Appliquer une optimisation possible pour obtenir la position et la taille d'un objet (tel que Shape). Les paramètres de hauteur de ligne et de largeur de colonne ne doivent pas être modifiés pendant l'accès optimisé. |
| [CellsData](./cellsdata/) | Appliquer une optimisation possible pour obtenir les valeurs des cellules. Les données des cellules (données et paramètres de Cell, Row) ne doivent pas être modifiés pendant l'accès optimisé, aucun nouvel objet Cell/Row ne doit être créé non plus (tel que par <see cref="Cells.this[int, int]"/>). |
| [CellDisplay](./celldisplay/) | Appliquer une optimisation possible pour obtenir les résultats liés à l'affichage des cellules (<see cref="Cell.DisplayStringValue"/>, <see cref="Cell.GetStyle()"/>, <see cref="Cell.GetDisplayStyle()"/>, etc.). Les données des cellules et les objets liés au style (styles Cell/Row/Column, largeur de colonne, etc.) ne doivent pas être modifiés pendant l'accès optimisé. |
| [GetFormula](./getformula/) | Appliquer une optimisation possible pour obtenir les formules. Toutes les données et paramètres pouvant affecter l'expression de la formule (nom de la feuille de calcul, texte du nom, colonne du tableau, etc.) ne doivent pas être modifiés pendant l'accès optimisé. |
| [SetFormula](./setformula/) | Appliquer une optimisation possible pour définir les formules. Toutes les données et paramètres pouvant affecter l'expression de la formule (nom de la feuille de calcul, texte du nom, colonne du tableau, etc.) ne doivent pas être modifiés pendant l'accès optimisé. |
| [CalculateFormula](./calculateformula/) | Appliquer une optimisation possible pour calculer les formules. Les données des cellules ne doivent pas être modifiées pendant l'accès optimisé, aucun nouvel objet (Cell, Row, etc.) ne doit être créé non plus (tel que par <see cref="Cells.this[int, int]"/>). |
| [ConditionalFormatting](./conditionalformatting/) | Appliquer une optimisation possible pour obtenir le résultat de formatage des mises en forme conditionnelles. Toutes les données et paramètres pouvant affecter le résultat des mises en forme conditionnelles (paramètres des mises en forme conditionnelles, valeurs des cellules dépendantes, etc.) ne doivent pas être modifiés pendant l'accès optimisé. |
| [Validation](./validation/) | Appliquer une optimisation possible pour obtenir le résultat de validation. Toutes les données et paramètres pouvant affecter le résultat de la validation (paramètres de la validation, valeurs des cellules dépendantes, etc.) ne doivent pas être modifiés pendant l'accès optimisé. |
