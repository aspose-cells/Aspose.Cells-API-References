---
title: "Validation.ErrorTitle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Validation. Représente le titre de la boîte de dialogue d'erreur de validation des données"
type: docs
url: /fr/net/aspose.cells/validation/errortitle/
---
## Validation.ErrorTitle property

Représente le titre de la boîte de dialogue d'erreur de validation des données.

```csharp
public string ErrorTitle { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyErrorTitleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Validation validation = worksheet.Validations[worksheet.Validations.Add(CellArea.CreateCellArea(0, 0, 1, 1))];
            
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "3";
            validation.Formula2 = "1234";
            
            validation.ErrorTitle = "Invalid Input";
            validation.ErrorMessage = "Value must be between 3 and 1234";
            validation.ShowError = true;

            workbook.Save("ValidationErrorTitleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


