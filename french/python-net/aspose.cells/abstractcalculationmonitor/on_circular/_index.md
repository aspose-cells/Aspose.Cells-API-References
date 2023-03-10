---
title: on_circular méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 40
url: /fr/python-net/aspose.cells/abstractcalculationmonitor/on_circular/
is_root: false
---
##  on_circular(circular_cells_data) {#collections.abc.Iterator}
Implémentez cette méthode pour faire des affaires lors du calcul de formules avec des références circulaires.


###  Retour

Indique si le moteur de formule doit calculer ces cellules en circulaire après cet appel.
True pour laisser le moteur de formule continuer à faire le calcul pour eux.
False pour laisser le moteur de formule simplement marquer ces cellules comme calculées.


```python
def on_circular(self, circular_cells_data):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| circular_cells_data | collections.abc.Iterator | IEnumerator avec des éléments CalculationCell représentant des cellules qui<br/> dépendent de références circulaires.|
###  Remarques

Dans l'implémentation, l'utilisateur peut également définir la valeur attendue comme résultat calculé
pour une partie/toutes ces cellules afin que le moteur de formule ne les calcule pas de manière récursive.


###  Voir également
* module [aspose.cells](../../)
* classe [AbstractCalculationMonitor](/cells/fr/python-net/aspose.cells/abstractcalculationmonitor)
