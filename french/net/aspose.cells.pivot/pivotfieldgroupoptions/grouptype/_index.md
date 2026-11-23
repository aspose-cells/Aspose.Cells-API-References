---
title: "PivotFieldGroupOptions.GroupType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotFieldGroupOptions. Obtient ou définit le type de regroupement pour le champ pivot. Seulement pour le regroupement des champs pivot de type date et heure"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfieldgroupoptions/grouptype/
---
## PivotFieldGroupOptions.GroupType property

Obtient ou définit le type de regroupement pour le champ du tableau croisé dynamique. Seulement pour le champ de date/heure.

```csharp
public PivotGroupByType GroupType { get; set; }
```

### Exemples

```csharp
//init
PivotFieldGroupOptions pivotFieldGroupOptions = new PivotFieldGroupOptions();
// Regrouper par année et mois ensemble
PivotGroupByType pivotGroupByType = pivotFieldGroupOptions.GroupType;
pivotGroupByType = PivotGroupByType.Years | PivotGroupByType.Months;
pivotFieldGroupOptions.GroupType = pivotGroupByType;
```

### Voir aussi

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotFieldGroupOptions](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


