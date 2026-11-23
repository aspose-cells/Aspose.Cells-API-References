---
title: "Classe Validation"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.GridWeb.Validation."
type: docs
url: /fr/net/aspose.cells.gridweb/validation/
---
## Validation class

```csharp
[Obsolete("This class is obsolete; use  GridValidation instead")]
public class Validation : CellAttachObject
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [Validation](validation/#constructor)() | Le constructeur par défaut. |
| [Validation](validation/#constructor_1)(GridValidation) |  |

## Propriétés

| Nom | Description |
| --- | --- |
| [Cell](../../aspose.cells.gridweb.data/cellattachobject/cell/) { get; } | Obtient la cellule relative de l'objet.(Héritée de [`CellAttachObject`](../../aspose.cells.gridweb.data/cellattachobject/).) |
| [ClientValidationFunction](../../aspose.cells.gridweb/validation/clientvalidationfunction/) { get; set; } | Obtient ou définit le nom de la fonction JavaScript de validation côté client. |
| [ClientValidationOpType](../../aspose.cells.gridweb/validation/clientvalidationoptype/) { get; set; } | Obtient ou définit le type d'opération de validation, Between/NotBetween/Equal/NotEqual/Greater/GreaterOrEqual/Less/LessOrEqual. |
| [ClientValidationValue1](../../aspose.cells.gridweb/validation/clientvalidationvalue1/) { get; set; } | Obtient ou définit la valeur cible de l'opérateur 1 |
| [ClientValidationValue2](../../aspose.cells.gridweb/validation/clientvalidationvalue2/) { get; set; } | Obtient ou définit la valeur cible de l'opérateur 2 |
| [IsRequired](../../aspose.cells.gridweb/validation/isrequired/) { get; set; } | Obtient ou définit si la valeur de la cellule est requise. |
| [RegEx](../../aspose.cells.gridweb/validation/regex/) { get; set; } | Obtient ou définit la chaîne d'expression régulière. |
| [ValueArray](../../aspose.cells.gridweb/validation/valuearray/) { get; set; } |  |
| [ValueList](../../aspose.cells.gridweb/validation/valuelist/) { get; } | Obtient l'objet liste de valeurs. |
| [ValueText](../../aspose.cells.gridweb/validation/valuetext/) { get; set; } | Utilisé uniquement en temps de conception. |

## Méthodes

| Nom | Description |
| --- | --- |
| [LoadValueList](../../aspose.cells.gridweb/validation/loadvaluelist/)(DataView, string, string, bool) | Charge la liste de valeurs à partir d'un objet DataView. Vous pouvez spécifier le champ de valeur et le champ de texte du DataView. Chaque paire valeur et texte sera combinée en une seule chaîne, séparée par une virgule. |

### Remarques

NOTE : Cette classe est maintenant obsolète. veuillez utiliser GridValidation à la place. Cette classe sera supprimée après 6 mois à compter d'août 2014. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Voir aussi

* class [CellAttachObject](../../aspose.cells.gridweb.data/cellattachobject/)
* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


