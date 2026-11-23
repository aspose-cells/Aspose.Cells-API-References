---
title: "Énumération ValidationAlertType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.ValidationAlertType. Représente le style d'alerte de validation des données"
type: docs
url: /fr/net/aspose.cells/validationalerttype/
---
## ValidationAlertType enumeration

Représente le style d'alerte de validation des données.

```csharp
public enum ValidationAlertType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Information | `0` | Style d'alerte d'information. |
| Stop | `1` | Style d'alerte d'arrêt. |
| Warning | `2` | Style d'alerte d'avertissement. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationAlertTypeDemo
    {
        public static void ValidationAlertTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir une zone de cellules pour la validation
            CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);

            // Ajouter une validation à la feuille de calcul
            ValidationCollection validations = worksheet.Validations;
            int validationIndex = validations.Add(area);
            Validation validation = validations[validationIndex];

            // Définir les propriétés de validation
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "3";
            validation.Formula2 = "1234";
            validation.AlertStyle = ValidationAlertType.Stop; // Using the ValidationAlertType enum
            validation.ErrorTitle = "Invalid Input";
            validation.ErrorMessage = "Please enter a number between 3 and 1234.";
            validation.ShowError = true;

            // Enregistrez le classeur
            workbook.Save("ValidationAlertTypeExample.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


