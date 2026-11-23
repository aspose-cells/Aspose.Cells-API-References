---
title: "Validation.Operator"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Validation. Représente l'opérateur pour la validation de données"
type: docs
url: /fr/net/aspose.cells/validation/operator/
---
## Validation.Operator property

Représente l'opérateur de la validation des données.

```csharp
public OperatorType Operator { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyOperatorDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour la validation
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Créer une plage de validation
            CellArea area = CellArea.CreateCellArea("B1", "B5");
            int validationIndex = worksheet.Validations.Add(area);
            Validation validation = worksheet.Validations[validationIndex];

            // Définir les propriétés de validation avec une démonstration de l'Operator
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "30";
            validation.ShowError = true;
            validation.ErrorMessage = "Value must be between 10 and 30";

            // Enregistrez le classeur
            workbook.Save("ValidationOperatorDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [OperatorType](../../operatortype/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


