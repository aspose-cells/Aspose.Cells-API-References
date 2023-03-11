---
title: keep_unparsed_data propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 120
url: /fr/python-net/aspose.cells/jsonloadoptions/keep_unparsed_data/
is_root: false
---
##  keep_unparsed_data propriété

Indique si les données non analysées sont conservées en mémoire pour le classeur lorsqu'il est chargé à partir du fichier de modèle. La valeur par défaut est true.

###  Remarques

Pour les scénarios où l'utilisateur n'a besoin que de lire certains contenus du fichier de modèle et n'a pas besoin de sauvegarder le classeur,
définir cette propriété sur false peut améliorer les performances, en particulier lors de son utilisation avec une sorte de LoadFilter,
###  Définition:
```python
@property
def keep_unparsed_data(self):
    ...
@keep_unparsed_data.setter
def keep_unparsed_data(self, value):
    ...
```

###  Voir également
* module [aspose.cells](../../)
* classe [JsonLoadOptions](/cells/fr/python-net/aspose.cells/jsonloadoptions)
