---
title: multi_thread_reading propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 1200
url: /fr/python-net/aspose.cells/cells/multi_thread_reading/
is_root: false
---
##  multi_thread_reading propriété

Obtient ou définit si le modèle de données des cellules doit prendre en charge la lecture multithread.
La valeur par défaut de cette propriété est false.

###  Remarques

S'il existe plusieurs threads pour lire simultanément les objets Row/Cell dans cette collection,
cette propriété doit être définie sur true, sinon un résultat inattendu peut être produit.
La prise en charge de la lecture multithread peut dégrader les performances d'accès aux objets Row/Cell de cette collection.
Veuillez noter que certaines fonctionnalités ne peuvent pas prendre en charge la lecture multi-thread,
telles que les valeurs de formatage (par [Cell.string_value](/cells/fr/python-net/aspose.cells/cell#string_value), [Cell.display_string_value](/cells/fr/python-net/aspose.cells/cell#display_string_value), .etc.).
Ainsi, même si cette propriété est définie sur true, ces API peuvent toujours donner un résultat inattendu pour la lecture multi-thread.
###  Définition:
```python
@property
def multi_thread_reading(self):
    ...
@multi_thread_reading.setter
def multi_thread_reading(self, value):
    ...
```

###  Voir également
* module [aspose.cells](../../)
* classe [Cells](/cells/fr/python-net/aspose.cells/cells)
