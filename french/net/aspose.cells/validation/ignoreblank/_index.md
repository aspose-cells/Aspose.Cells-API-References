---
title: "Validation.IgnoreBlank"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Validation. Indique si les valeurs vides sont autorisées par la validation de données de la plage"
type: docs
url: /fr/net/aspose.cells/validation/ignoreblank/
---
## Validation.IgnoreBlank property

Indique si les valeurs vides sont autorisées par la validation de plage de données.

```csharp
public bool IgnoreBlank { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyIgnoreBlankDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            ValidationCollection validations = sheet.Validations;
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 1;
            area.StartColumn = 0;
            area.EndColumn = 1;
            Validation validation = validations[validations.Add(area)];

            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "2";
            validation.Formula2 = "20";
            validation.IgnoreBlank = true;

            Console.WriteLine("Validation created with IgnoreBlank set to: " + validation.IgnoreBlank);
        }
    }
}
```

### Voir aussi

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


