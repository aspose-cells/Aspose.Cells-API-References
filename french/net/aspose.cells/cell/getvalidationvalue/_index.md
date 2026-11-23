---
title: "Cell.GetValidationValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cell. Obtient la valeur de validation appliquée à cette cellule"
type: docs
url: /fr/net/aspose.cells/cell/getvalidationvalue/
---
## Cell.GetValidationValue method

Obtient la valeur de validation appliquée à cette cellule.

```csharp
public bool GetValidationValue()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetValidationValueDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une plage de validation
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.TextLength;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "1";
            validation.Formula2 = "5";

            // Appliquer la validation à la cellule A1
            Cell cell = worksheet.Cells["A1"];
            validation.AddArea(new CellArea { StartRow = cell.Row, StartColumn = cell.Column, EndRow = cell.Row, EndColumn = cell.Column });

            // Tester les valeurs valides
            string[] validValues = { "a", " ab", "cd ", " xyz " };
            foreach (string value in validValues)
            {
                cell.PutValue(value);
                Console.WriteLine($"Value: '{value}' - Valid: {cell.GetValidationValue()}");
            }

            // Tester la valeur invalide
            string invalidValue = "toolong";
            cell.PutValue(invalidValue);
            Console.WriteLine($"Value: '{invalidValue}' - Valid: {cell.GetValidationValue()}");
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


