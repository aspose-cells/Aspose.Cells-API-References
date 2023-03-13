---
title: start_access_cache méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 380
url: /fr/python-net/aspose.cells/workbook/start_access_cache/
is_root: false
---
##  start_access_cache(opts) {#AccessCacheOptions}
Démarre la session qui utilise les caches pour accéder aux données.



```python
def start_access_cache(self, opts):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| opts | [AccessCacheOptions](/cells/fr/python-net/aspose.cells/accesscacheoptions) | options d'accès aux données|
###  Remarques

Si le cache de l'accès aux données spécifié nécessite que certains modèles de données dans la feuille de calcul soient "en lecture seule",
alors les modèles de données correspondants dans chaque feuille de calcul de ce classeur seront considérés comme "en lecture seule"
et l'utilisateur ne doit en modifier aucun.


Après avoir terminé l'accès aux données, [Workbook.close_access_cache(opts)](/cells/fr/python-net/aspose.cells/workbook/close_access_cache) devrait
être invoqué avec les mêmes options pour effacer tous les caches et récupérer le mode d'accès normal.


###  Voir également
* module [aspose.cells](../../)
* classe [Workbook](/cells/fr/python-net/aspose.cells/workbook)
