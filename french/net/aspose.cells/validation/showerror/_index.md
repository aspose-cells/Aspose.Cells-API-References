---
title: "Validation.ShowError"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Validation. Indique si le message d'erreur de validation des données sera affiché chaque fois que l'utilisateur saisit des données invalides"
type: docs
url: /fr/net/aspose.cells/validation/showerror/
---
## Validation.ShowError property

Indique si le message d'erreur de validation des données sera affiché chaque fois que l'utilisateur saisit des données invalides.

```csharp
public bool ShowError { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyShowErrorDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une validation pour la cellule A1
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });
            
            // Définir les propriétés de validation
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "20";
            
            // Configurer l'alerte d'erreur
            validation.ShowError = true;
            validation.ErrorTitle = "Invalid Input";
            validation.ErrorMessage = "Value must be between 10 and 20";

            // Créer une autre validation pour démontrer la copie de propriétés
            Validation targetValidation = worksheet.Validations[worksheet.Validations.Add()];
            targetValidation.AddArea(new CellArea { StartRow = 1, StartColumn = 0, EndRow = 1, EndColumn = 0 });

            // Copier ShowError et les propriétés associées de la première validation
            targetValidation.ShowError = validation.ShowError;
            targetValidation.ErrorTitle = validation.ErrorTitle;
            targetValidation.ErrorMessage = validation.ErrorMessage;

            // Enregistrez le classeur
            workbook.Save("ValidationShowErrorDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


