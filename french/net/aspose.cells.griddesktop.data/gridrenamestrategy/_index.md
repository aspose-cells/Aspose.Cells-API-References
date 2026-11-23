---
title: "Enum GridRenameStrategy"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.GridDesktop.Data.GridRenameStrategy enum. Option de stratégie pour les noms de colonnes en double"
type: docs
url: /fr/net/aspose.cells.griddesktop.data/gridrenamestrategy/
---
## GridRenameStrategy enumeration

Option de stratégie pour les noms de colonnes en double.

```csharp
public enum GridRenameStrategy
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Exception | `0` | Lance une exception. |
| Digit | `1` | Nommé avec un chiffre. Les noms dupliqués deviendront ...1, ...2, etc. |
| Letter | `2` | Nommé avec une lettre.. Les noms dupliqués deviendront ...A, ...B, etc. |

### Remarques

Lors du traitement des données avec des en-têtes, certains scénarios exigent que les en-têtes ne soient pas dupliqués pour toutes les colonnes. Par exemple, lors de l'exportation de données vers un DataTable et que l'en-tête doit être utilisé comme nom de colonne du DataTable, les valeurs d'en-tête dupliquées sont invalides. Dans ce type de situation, l'utilisateur peut déterminer comment les gérer en spécifiant cette stratégie.

### Voir aussi

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


