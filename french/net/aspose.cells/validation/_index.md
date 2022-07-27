---
title: Validation
second_title: Référence de l'API Aspose.Cells pour .NET
description: Représente la validation des données.settings.
type: docs
weight: 6200
url: /fr/net/aspose.cells/validation/
---
## Validation class

Représente la validation des données.settings.

```csharp
public class Validation
```

## Propriétés

| Nom | La description |
| --- | --- |
| [AlertStyle](../../aspose.cells/validation/alertstyle) { get; set; } | Représente le style d'alerte de validation. |
| [Areas](../../aspose.cells/validation/areas) { get; } | Obtient tout[`CellArea`](../cellarea) qui contiennent les paramètres de validation des données. |
| [ErrorMessage](../../aspose.cells/validation/errormessage) { get; set; } | Représente le message d'erreur de validation des données. |
| [ErrorTitle](../../aspose.cells/validation/errortitle) { get; set; } | Représente le titre de la boîte de dialogue d'erreur de validation des données. |
| [Formula1](../../aspose.cells/validation/formula1) { get; set; } | Représente la valeur ou l'expression associée à la validation des données. |
| [Formula2](../../aspose.cells/validation/formula2) { get; set; } | Représente la valeur ou l'expression associée à la validation des données. |
| [IgnoreBlank](../../aspose.cells/validation/ignoreblank) { get; set; } | Indique si les valeurs vides sont autorisées par la validation des données de plage. |
| [InCellDropDown](../../aspose.cells/validation/incelldropdown) { get; set; } | Indique si la validation des données affiche une liste déroulante contenant des valeurs acceptables. |
| [InputMessage](../../aspose.cells/validation/inputmessage) { get; set; } | Représente le message d'entrée de validation des données. |
| [InputTitle](../../aspose.cells/validation/inputtitle) { get; set; } | Représente le titre de la boîte de dialogue d'entrée de validation des données. |
| [Operator](../../aspose.cells/validation/operator) { get; set; } | Représente l'opérateur pour la validation des données. |
| [ShowError](../../aspose.cells/validation/showerror) { get; set; } | Indique si le message d'erreur de validation des données s'affichera chaque fois que l'utilisateur saisira des données non valides. |
| [ShowInput](../../aspose.cells/validation/showinput) { get; set; } | Indique si le message d'entrée de validation des données sera affiché chaque fois que l'utilisateur sélectionne une cellule dans la plage de validation des données. |
| [Type](../../aspose.cells/validation/type) { get; set; } | Représente le type de validation des données. |
| [Value1](../../aspose.cells/validation/value1) { get; set; } | Représente la première valeur associée à la validation des données. |
| [Value2](../../aspose.cells/validation/value2) { get; set; } | Représente la deuxième valeur associée à la validation des données. |

## Méthodes

| Nom | La description |
| --- | --- |
| [AddArea](../../aspose.cells/validation/addarea#addarea)(CellArea) | Applique la validation à la zone. |
| [AddArea](../../aspose.cells/validation/addarea#addarea_1)(CellArea, bool, bool) | Applique la validation à la zone. |
| [AddAreas](../../aspose.cells/validation/addareas)(CellArea[], bool, bool) | Applique la validation à des zones données. |
| [Copy](../../aspose.cells/validation/copy)(Validation, CopyOptions) | Validation de la copie. |
| [GetFormula1](../../aspose.cells/validation/getformula1#getformula1)(bool, bool) | Obtient la valeur ou l'expression associée à cette validation. |
| [GetFormula1](../../aspose.cells/validation/getformula1#getformula1_1)(bool, bool, int, int) | Obtient la valeur ou l'expression associée à cette validation pour une cellule spécifique. |
| [GetFormula2](../../aspose.cells/validation/getformula2#getformula2)(bool, bool) | Obtient la valeur ou l'expression associée à cette validation. |
| [GetFormula2](../../aspose.cells/validation/getformula2#getformula2_1)(bool, bool, int, int) | Obtient la valeur ou l'expression associée à cette validation pour une cellule spécifique. |
| [GetListValue](../../aspose.cells/validation/getlistvalue)(int, int) | Obtenir la valeur de la liste de validation pour la cellule spécifiée. |
| [RemoveACell](../../aspose.cells/validation/removeacell)(int, int) | Supprimer les paramètres de validation dans la cellule. |
| [RemoveArea](../../aspose.cells/validation/removearea)(CellArea) | Supprimez les paramètres de validation dans la plage. |
| [RemoveAreas](../../aspose.cells/validation/removeareas)(CellArea[]) | Supprime cette validation des zones données. |
| [SetFormula1](../../aspose.cells/validation/setformula1)(string, bool, bool) | Définit la valeur ou l'expression associée à cette validation. |
| [SetFormula2](../../aspose.cells/validation/setformula2)(string, bool, bool) | Définit la valeur ou l'expression associée à cette validation. |

### Exemples

```csharp
[C#]
Workbook workbook = new Workbook();
ValidationCollection validations = workbook.Worksheets[0].Validations;
CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);
Validation validation = validations[validations.Add(area)];
validation.Type = Aspose.Cells.ValidationType.WholeNumber;
validation.Operator = OperatorType.Between;
validation.Formula1 = "3";
validation.Formula2 = "1234";

[Visual Basic]
Dim workbook as Workbook = new Workbook()
Dim validations as ValidationCollection  = workbook.Worksheets(0).Validations
Dim area as CellArea = CellArea.CreateCellArea(0, 0, 1, 1);
Dim validation as Validation = validations(validations.Add(area))
validation.Type = ValidationType.WholeNumber
validation.Operator = OperatorType.Between
validation.Formula1 = "3"
validation.Formula2 = "1234"
```

### Voir également

* espace de noms [Aspose.Cells](../../aspose.cells)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
