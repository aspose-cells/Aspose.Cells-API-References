---
title: "GridDesktop.AlwasysRecalculateAllFormulas"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "GridDesktop propriété. Obtient ou définit une valeur indiquant si nous devons exécuter toutes les formules comme lorsque nous exécutons toutes les formules lors de la mise à jour de la valeur d'une cellule et que cela affecte d'autres cellules, qui à leur tour affectent d'autres cellules, de plus en plus, car toutes les cellules doivent être recalculées, à l'instar de l'effet papillon. Cela nécessite de nombreuses opérations de pile, ce qui entraîne de très faibles performances, comme dans CELLSNET41921. Ce problème contient le fichier qui peut illustrer ce scénario où il vaut mieux exécuter toutes les formules, car lorsque nous exécutons toutes les formules nous pouvons avoir certaines optimisations."
type: docs
url: /fr/net/aspose.cells.griddesktop/griddesktop/alwasysrecalculateallformulas/
---
## GridDesktop.AlwasysRecalculateAllFormulas property

Obtient ou définit une valeur indiquant si nous devons exécuter toutes les formules, comme lorsque nous exécutons toutes les formules, lorsqu'une valeur de cellule est mise à jour et qu'elle affecte d'autres cellules, qui à leur tour affectent d'autres cellules, etc., entraînant le recalcul de toutes les cellules, à l'instar de l'effet papillon. Cela nécessite de nombreuses opérations de pile, ce qui entraîne de très faibles performances, comme dans CELLSNET-41921. Ce problème contient le fichier qui illustre ce scénario ; il vaut mieux simplement exécuter toutes les formules, car lorsque toutes les formules sont exécutées nous pouvons avoir certaines optimisations.

```csharp
public bool AlwasysRecalculateAllFormulas { get; set; }
```

### Voir aussi

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


