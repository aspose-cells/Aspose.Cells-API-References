---
title: StartAccessCache
second_title: Référence de l'API Aspose.Cells pour .NET
description: Démarre la session qui utilise les caches pour accéder aux données.
type: docs
weight: 630
url: /fr/net/aspose.cells/workbook/startaccesscache/
---
## Workbook.StartAccessCache method

Démarre la session qui utilise les caches pour accéder aux données.

```csharp
public void StartAccessCache(AccessCacheOptions opts)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| opts | AccessCacheOptions | options d'accès aux données |

### Remarques

Si le cache de l'accès aux données spécifié nécessite que certains modèles de données dans la feuille de calcul soient en "lecture seule", , les modèles de données correspondants dans chaque feuille de calcul de ce classeur seront considérés comme "en lecture seule" et l'utilisateur ne doit en modifier aucun. .  Après avoir terminé l'accès aux données,[`CloseAccessCache`](../closeaccesscache) devrait être invoqué avec les mêmes options pour effacer tous les caches et récupérer le mode d'accès normal.

### Voir également

* enum [AccessCacheOptions](../../accesscacheoptions)
* class [Workbook](../../workbook)
* espace de noms [Aspose.Cells](../../workbook)
* Assemblée [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
