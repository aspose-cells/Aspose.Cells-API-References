---
title: "GridCell.CreateValidation"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode GridCell. Crée un objet de validation pour une cellule"
type: docs
url: /fr/net/aspose.cells.gridweb.data/gridcell/createvalidation/
---
## GridCell.CreateValidation method

Crée un objet de validation pour une cellule.

```csharp
public GridValidation CreateValidation(GridValidationType validationType, bool isRequried)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| validationType | GridValidationType | Type de validation. |
| isRequried | Boolean | Indique si la valeur de la cellule est requise. |

### Exemples

```csharp
[C#]
GridWeb GridWeb1 = new GridWeb();
GridWorksheet sheet = GridWeb1.ActiveSheet;
GridValidation v = sheet.Cells["A1"].CreateValidation(GridValidationType.CustomExpression, true);
	// Définit l'expression de validation numérique.
	v.RegEx = "\\d+";
	
[Visual Basic]
im GridWeb1 As GridWeb =  New GridWeb() 
im sheet As GridWorksheet =  GridWeb1.ActiveSheet 
	Dim v As GridValidation =  sheet.Cells["A1"].CreateValidation(GridValidationType.CustomExpression,True) 
	 ' Sets to number validation expression.
	v.RegEx = "\\d+"
```

### Voir aussi

* class [GridValidation](../../gridvalidation/)
* enum [GridValidationType](../../gridvalidationtype/)
* class [GridCell](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


