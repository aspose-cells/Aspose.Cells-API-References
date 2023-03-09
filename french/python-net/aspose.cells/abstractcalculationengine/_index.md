---
title: AbstractCalculationEngine classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 20
url: /fr/python-net/aspose.cells/abstractcalculationengine/
is_root: false
---
##  AbstractCalculationEngine classe
Représente le moteur de calcul personnalisé de l'utilisateur pour étendre le moteur de calcul par défaut de Aspose.Cells.



Le type AbstractCalculationEngine expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [is_param_literal_required](/cells/fr/python-net/aspose.cells/abstractcalculationengine/is_param_literal_required) | Indique si ce moteur a besoin du texte littéral du paramètre lors du calcul. La valeur par défaut est faux.|
| [process_built_in_functions](/cells/fr/python-net/aspose.cells/abstractcalculationengine/process_built_in_functions) | Si les fonctions intégrées qui ont été prises en charge par le moteur intégré doivent être vérifiées et traitées par cette implémentation.<br/>La valeur par défaut est false.<br/>Si l'utilisateur doit modifier la logique de calcul de certaines fonctions intégrées, cette propriété doit être définie sur true.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [calculate(data)](/cells/fr/python-net/aspose.cells/abstractcalculationengine/calculate/#CalculationData) | Calcule une fonction avec des données données.|



###  Remarques

L'utilisateur ne doit modifier aucune partie du classeur directement dans cette implémentation (à l'exception du résultat calculé de la fonction personnalisée, qui peut être défini par la propriété CalculationData.CalculatedValue).
Sinon, un résultat inattendu ou une exception peut être causé.
Si l'utilisateur a besoin de modifier d'autres données que le résultat calculé dans la mise en œuvre de certaines fonctions personnalisées,
par exemple, modifier la formule, le style, etc. de la cellule, l'utilisateur doit rassembler ces données dans cette implémentation et les modifier en dehors de la portée du calcul de la formule.

###  Voir également
* module [aspose.cells](..)
