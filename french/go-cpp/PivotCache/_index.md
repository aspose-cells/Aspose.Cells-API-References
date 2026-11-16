---
title: "Classe PivotCache"
linktitle: "PivotCache"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe PivotCache. Encapsule l'objet qui représente pivotcache en Go."
type: docs
weight: 200
url: /fr/go-cpp/pivotcache/
---

## PivotCache class

Représente le cache mémoire pour certains rapports de tableau croisé dynamique.

```go

type PivotCache struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetMissingItemsLimit](./getmissingitemslimit/) | Obtient et définit le nombre d'éléments inutilisés à autoriser avant de supprimer les éléments inutilisés. Cette valeur DOIT être supérieure à -2 et inférieure à 1048577. PivotCacheMissingItemsLimitConst; |
| [SetMissingItemsLimit](./setmissingitemslimit/) | Obtient et définit le nombre d'éléments inutilisés à autoriser avant de supprimer les éléments inutilisés. Cette valeur DOIT être supérieure à -2 et inférieure à 1048577. PivotCacheMissingItemsLimitConst; |
| [Refresh_PivotTableRefreshOption](./refresh_pivottablerefreshoption/) | Actualise les données de la source de données et calcule les données pour la vue de tous les pivottables dont la source de données est ce pivot cache. |
| [Refresh](./refresh/) | Actualise les données de la source de données et calcule les données pour la vue de tous les pivottables dont la source de données est ce pivot cache. |
| [GetPivotTables](./getpivottables/) | Obtient toutes les tables pivot avec ce cache de pivot. |
| [Dispose](./dispose/) | Libère toutes les ressources. |
| [GetSourceType](./getsourcetype/) | Obtient le PivotTableSourceType. |
