---
title: CalculationPrecisionStrategy dénombrement
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 1820
url: /fr/python-net/aspose.cells/calculationprecisionstrategy/
is_root: false
---
##  CalculationPrecisionStrategy dénombrement
Énumère les stratégies de gestion de la précision des calculs.
En raison du problème de précision de l'arithmétique à virgule flottante IEEE 754, certaines formules "apparemment simples" peuvent ne pas être calculées comme le résultat attendu.
Comme la formule "=-0.45+0.43+0.02", lors du calcul direct des opérandes par l'opérateur '+', le résultat n'est pas nul. Pour ce genre de problème de précision,
certaines stratégies spéciales peuvent donner le résultat escompté.



Le type CalculationPrecisionStrategy expose les membres suivants :

###  Des champs
| Champ| Description|
| :- | :- |
| NONE | Aucune stratégie appliquée sur le calcul.<br/>Lors du calcul, utilisez simplement la valeur double d'origine comme opérande et renvoyez directement le résultat.<br/> Le plus efficace pour les performances et applicable dans la plupart des cas.|
| ROUND | Arrondit le résultat du calcul en fonction des chiffres significatifs.|
| DECIMAL | Utilise décimal comme opérandes lorsque cela est possible.<br/> Le plus inefficace pour la performance.|



###  Voir également
* module [aspose.cells](..)
