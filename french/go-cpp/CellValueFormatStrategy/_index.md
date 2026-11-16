---
title: "CellValueFormatStrategy Enum"
linktitle: "CellValueFormatStrategy"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "CellValueFormatStrategy enum. Encapsule l'objet qui représente cellvalueformatstrategy en Go."
type: docs
weight: 200
url: /fr/go-cpp/cellvalueformatstrategy/
---

## CellValueFormatStrategy Enum

Spécifie comment appliquer le style à la valeur de la cellule.

```go

type CellValueFormatStrategy int32


```

## Champs

| Champ | Description |
| --- | --- |
| [None](./none/) | Non formaté. |
| [CellStyle](./cellstyle/) | Uniquement formaté avec le style original de la cellule. |
| [DisplayStyle](./displaystyle/) | Formaté avec le style affiché de la cellule. |
| [DisplayString](./displaystring/) | Obtient la chaîne affichée dans MS Excel. La principale différence avec <see cref="DisplayStyle"/> est que cette option prend également en compte l'effet de la largeur de colonne. Si la largeur de colonne est trop petite pour afficher complètement la chaîne formatée, "#" peut être affiché, comme le fait MS Excel. |
