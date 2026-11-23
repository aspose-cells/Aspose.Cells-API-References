---
title: "Enum ValidationType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.ValidationType enum. Représente le type de validation des données"
type: docs
url: /fr/net/aspose.cells/validationtype/
---
## ValidationType enumeration

Représente le type de validation des données.

```csharp
public enum ValidationType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| AnyValue | `0` | Type de validation de toute valeur. |
| WholeNumber | `1` | Type de validation de nombre entier. |
| Decimal | `2` | Type de validation décimal. |
| List | `3` | Type de validation de liste. |
| Date | `4` | Type de validation de date. |
| Time | `5` | Type de validation d'heure. |
| TextLength | `6` | Type de validation de longueur de texte. |
| Custom | `7` | Type de validation personnalisé. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationTypeDemo
    {
        public static void ValidationTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une validation à la feuille de calcul
            ValidationCollection validations = worksheet.Validations;
            CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);
            Validation validation = validations[validations.Add(area)];

            // Définir le type de validation sur WholeNumber
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "3";
            validation.Formula2 = "1234";

            // Définir des propriétés supplémentaires pour la validation
            validation.InputMessage = "Please enter a whole number between 3 and 1234.";
            validation.InputTitle = "Whole Number Validation";
            validation.ErrorMessage = "The value must be a whole number between 3 and 1234.";
            validation.ErrorTitle = "Invalid Input";
            validation.ShowInput = true;
            validation.ShowError = true;

            // Enregistrez le classeur
            workbook.Save("ValidationTypeExample.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


