---
title: "LookInType Enum"
linktitle: "LookInType"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "LookInType enum. Encapsule l'objet qui représente lookintype en Go."
type: docs
weight: 200
url: /fr/go-cpp/lookintype/
---

## LookInType Enum

Représente le type de look-in.

```go

type LookInType int32


```

## Champs

| Champ | Description |
| --- | --- |
| [Formulas](./formulas/) | Recherche l'objet recherché à partir de la formule(<see cref="Cell.Formula"/>) si la cellule est une formule, sinon recherche à partir de la valeur originale de la cellule (identique à <see cref="OriginalValues"/>). |
| [Values](./values/) | Recherche l'objet à partir de la valeur originale de la cellule(<see cref="Cell.Value"/>) et de la valeur formatée(<see cref="Cell.StringValue"/>). |
| [ValuesExcludeFormulaCell](./valuesexcludeformulacell/) | Ignore les cellules qui sont des formules. Pour les cellules qui ne sont pas des formules, c'est identique à <see cref="Values"/>. |
| [Comments](./comments/) | Recherche l'objet uniquement à partir du commentaire de la cellule. Ignore les cellules qui n'ont pas de commentaire. |
| [OnlyFormulas](./onlyformulas/) | Ignore les cellules qui ne sont pas des formules. Pour les cellules qui sont des formules, recherche l'objet recherché à partir de la formule(<see cref="Cell.Formula"/>). |
| [OriginalValues](./originalvalues/) | Recherche l'objet uniquement à partir de la valeur originale de la cellule. |
| [FormattedValues](./formattedvalues/) | Recherche l'objet uniquement à partir de la valeur formatée de la cellule(<see cref="Cell.StringValue"/>). |
