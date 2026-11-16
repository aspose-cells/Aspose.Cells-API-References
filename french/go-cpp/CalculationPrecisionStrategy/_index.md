---
title: "Enumération CalculationPrecisionStrategy"
linktitle: "CalculationPrecisionStrategy"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "CalculationPrecisionStrategy enum. Encapsule l'objet qui représente calculationprecisionstrategy en Go."
type: docs
weight: 200
url: /fr/go-cpp/calculationprecisionstrategy/
---

## CalculationPrecisionStrategy Enum

Énumère les stratégies de gestion de la précision de calcul.Parce au problème de précision de l’arithmétique à virgule flottante IEEE 754, certaines formules "apparemment simples" peuvent ne pas être calculées comme le résultat attendu.Par exemple la formule "=-0.45+0.43+0.02", lorsqu’on calcule les opérandes avec l’opérateur '+' directement, le résultat n’est pas zéro. Pour ce type de problème de précision, certaines stratégies spéciales peuvent fournir le résultat attendu.

```go

type CalculationPrecisionStrategy int32


```

## Champs

| Champ | Description |
| --- | --- |
| [None](./none/) | Aucune stratégie appliquée au calcul.Lors du calcul, utilisez simplement la valeur double originale comme opérande et renvoyez le résultat directement.Le plus efficace en termes de performances et applicable dans la plupart des cas. |
| [Round](./round/) | Arrondit le résultat du calcul selon les chiffres significatifs. |
| [Decimal](./decimal/) | Utilise le décimal comme opérandes lorsque possible.Le plus inefficace en termes de performances. |
