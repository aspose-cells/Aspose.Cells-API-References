---
title: "AbstractCalculationMonitor.BeforeCalculate"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode AbstractCalculationMonitor. Implémentez cette méthode pour effectuer des opérations avant de calculer une cellule"
type: docs
url: /fr/net/aspose.cells/abstractcalculationmonitor/beforecalculate/
---
## AbstractCalculationMonitor.BeforeCalculate method

Implémentez cette méthode pour effectuer des opérations avant le calcul d'une cellule.

```csharp
public virtual void BeforeCalculate(int sheetIndex, int rowIndex, int colIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sheetIndex | Int32 | Index de la feuille à laquelle la cellule appartient. |
| rowIndex | Int32 | Index de ligne de la cellule |
| colIndex | Int32 | Indice de colonne de la cellule |

### Remarques

Pour les cellules dans les formules de tableau, cette méthode peut ne pas être exécutée car généralement ces cellules sont calculées ensemble.

### Voir aussi

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


