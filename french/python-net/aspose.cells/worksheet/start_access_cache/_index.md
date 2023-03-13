---
title: start_access_cache méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 280
url: /fr/python-net/aspose.cells/worksheet/start_access_cache/
is_root: false
---
##  start_access_cache(opts) {#AccessCacheOptions}
Démarre la session qui utilise des caches pour accéder aux données de cette feuille de calcul.



```python
def start_access_cache(self, opts):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| opts | [AccessCacheOptions](/cells/fr/python-net/aspose.cells/accesscacheoptions) | options d'accès aux données|
###  Remarques

Après avoir terminé l'accès aux données, [Worksheet.close_access_cache(opts)](/cells/fr/python-net/aspose.cells/worksheet/close_access_cache) devrait
être invoqué avec les mêmes options pour effacer tous les caches et récupérer le mode d'accès normal.


###  Voir également
* module [aspose.cells](../../)
* classe [Worksheet](/cells/fr/python-net/aspose.cells/worksheet)
