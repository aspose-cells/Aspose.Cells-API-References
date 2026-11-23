---
title: "GridValidation.GetListValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode GridValidation. Obtient la valeur de la liste de validation pour la cellule spécifiée"
type: docs
url: /fr/net/aspose.cells.gridweb.data/gridvalidation/getlistvalue/
---
## GridValidation.GetListValue method

Obtenez la valeur de la liste de validation pour la cellule spécifiée.

```csharp
public object GetListValue(int row, int column)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | L'index de ligne. |
| column | Int32 | L'index de colonne. |

### Valeur de retour

La valeur permettant de produire la liste de cette validation pour la cellule spécifiée. Si la liste fait référence à une plage, la valeur retournée sera un objet ReferredArea ; sinon la valeur retournée peut être null, object[] ou un objet simple.

### Remarques

Uniquement pour les validations dont le type est List et qui ont été appliquées à la cellule donnée, sinon null sera retourné.

### Voir aussi

* class [GridValidation](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


