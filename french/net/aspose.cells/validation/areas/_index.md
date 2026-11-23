---
title: "Validation.Areas"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Validation. Obtient toutes les CellArea qui contiennent les paramètres de validation des données"
type: docs
url: /fr/net/aspose.cells/validation/areas/
---
## Validation.Areas property

Obtient toutes les [`CellArea`](../../cellarea/) qui contiennent les paramètres de validation des données.

```csharp
public CellArea[] Areas { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyAreasDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets.Add("Areas & rent");

            // Créer une validation pour la colonne A
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "1";
            validation.Formula2 = "100";

            // Ajouter des zones de validation à différentes lignes
            validation.AddArea(new CellArea { StartRow = 46, StartColumn = 0, EndRow = 50, EndColumn = 0 });
            validation.AddArea(new CellArea { StartRow = 92, StartColumn = 0, EndRow = 96, EndColumn = 0 });
            validation.AddArea(new CellArea { StartRow = 138, StartColumn = 0, EndRow = 142, EndColumn = 0 });

            // Démontrer l'accès aux zones de validation
            CellArea area1 = (CellArea)validation.Areas[0];
            Console.WriteLine($"Area 1 StartRow: {area1.StartRow}"); // Output: 46
            
            CellArea area2 = (CellArea)validation.Areas[1];
            Console.WriteLine($"Area 2 StartRow: {area2.StartRow}"); // Output: 92
            
            CellArea area3 = (CellArea)validation.Areas[2];
            Console.WriteLine($"Area 3 StartRow: {area3.StartRow}"); // Output: 138
        }
    }
}
```

### Voir aussi

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


