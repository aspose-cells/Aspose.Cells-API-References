---
title: "PivotField.Subtotals"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotField. Obtient ou définit les sous‑totaux du champ. Seulement pour les champs pivot de ligne ou de colonne"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/subtotals/
---
## PivotField.Subtotals property

Obtient ou définit les sous‑totaux du champ. Seulement pour les champs pivot de ligne ou de colonne.

```csharp
public PivotFieldSubtotalType Subtotals { get; set; }
```

### Exemples

```csharp

[C#]
//Pas de sous‑totaux
rowField.Subtotals = PivotFieldSubtotalType.None;
//Sous‑totaux automatiques
//rowField.Subtotals = PivotFieldSubtotalType.Automatic;
//Sous‑totaux uniques : Somme
//rowField.Subtotals = PivotFieldSubtotalType.Sum;
//Sous‑totaux multiples : Somme et comptage des nombres
//rowField.Subtotals = PivotFieldSubtotalType.Sum | PivotFieldSubtotalType.Count;
```

### Voir aussi

* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


