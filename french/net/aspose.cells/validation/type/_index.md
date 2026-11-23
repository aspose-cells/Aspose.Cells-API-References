---
title: "Validation.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Validation. Représente le type de validation des données"
type: docs
url: /fr/net/aspose.cells/validation/type/
---
## Validation.Type property

Représente le type de validation des données.

```csharp
public ValidationType Type { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une validation à la cellule A1
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.ErrorTitle = "Number Validation";
            validation.ErrorMessage = "Please enter a whole number";
            validation.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });

            // Démontrer la propriété Type
            Console.WriteLine("Validation Type: " + validation.Type);
            
            // Enregistrez le classeur
            workbook.Save("ValidationExample.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ValidationType](../../validationtype/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


