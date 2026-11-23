---
title: "Worksheet.Validations"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Worksheet. Obtient la collection des paramètres de validation des données dans la feuille de calcul"
type: docs
url: /fr/net/aspose.cells/worksheet/validations/
---
## Worksheet.Validations property

Obtient la collection des paramètres de validation des données dans la feuille de calcul.

```csharp
public ValidationCollection Validations { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyValidationsDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une validation de données à la cellule A1
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.List;
            validation.Formula1 = "Option1,Option2,Option3";
            
            // Correction : créer CellArea avec StartRow, StartColumn, EndRow, EndColumn
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            validation.AddArea(area);

            // Obtenir la validation de la cellule A1
            Validation cellValidation = worksheet.Validations.GetValidationInCell(0, 0);
            
            // Afficher le type de validation
            Console.WriteLine("Validation type in A1: " + cellValidation.Type);
            
            // Enregistrez le classeur
            workbook.Save("ValidationDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ValidationCollection](../../validationcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


