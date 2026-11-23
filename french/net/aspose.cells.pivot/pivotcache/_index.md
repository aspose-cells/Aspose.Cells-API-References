---
title: "Classe PivotCache"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Pivot.PivotCache. Représente le cache mémoire pour certains rapports de PivotTable"
type: docs
url: /fr/net/aspose.cells.pivot/pivotcache/
---
## PivotCache class

Représente le cache mémoire pour certains rapports de tableau croisé dynamique.

```csharp
public abstract class PivotCache : IDisposable
```

## Propriétés

| Nom | Description |
| --- | --- |
| [MissingItemsLimit](../../aspose.cells.pivot/pivotcache/missingitemslimit/) { get; set; } | Obtient et définit le nombre d’éléments inutilisés à autoriser avant de supprimer les éléments inutilisés. Cette valeur DOIT être supérieure à -2 et inférieure à 1048577. [`PivotCacheMissingItemsLimitConst`](../pivotcachemissingitemslimitconst/); |
| abstract [SourceType](../../aspose.cells.pivot/pivotcache/sourcetype/) { get; } | Obtient le [`PivotTableSourceType`](../pivottablesourcetype/). |

## Méthodes

| Nom | Description |
| --- | --- |
| abstract [Dispose](../../aspose.cells.pivot/pivotcache/dispose/)() | Libérez toutes les ressources. |
| [GetPivotTables](../../aspose.cells.pivot/pivotcache/getpivottables/)() | Obtient tous les tableaux croisés dynamiques avec ce cache de tableau croisé dynamique. |
| [Refresh](../../aspose.cells.pivot/pivotcache/refresh/#refresh)() | Actualise les données depuis la source de données et calcule les données pour la vue de tous les tableaux croisés dynamiques dont la source de données est ce cache de tableau croisé dynamique. |
| [Refresh](../../aspose.cells.pivot/pivotcache/refresh/#refresh_1)(PivotTableRefreshOption) | Actualise les données depuis la source de données et calcule les données pour la vue de tous les tableaux croisés dynamiques dont la source de données est ce cache de tableau croisé dynamique. |

### Remarques

Toutes les données seront rassemblées dans ce cache, et le tableau croisé dynamique ne récupère les données que depuis ce cache, sans accéder directement à la source de données. Si la source de données de certains [`PivotTable`](../pivottable/) est la même, ils utiliseront un cache de tableau croisé dynamique.

### Voir aussi

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


