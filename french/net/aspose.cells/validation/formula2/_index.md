---
title: "Validation.Formula2"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Validation. Représente la valeur ou l'expression associée à la validation des données"
type: docs
url: /fr/net/aspose.cells/validation/formula2/
---
## Validation.Formula2 property

Représente la valeur ou l'expression associée à la validation des données.

```csharp
public string Formula2 { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyFormula2Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            sheet.Cells["B3"].PutValue(100);
            sheet.Cells["B7"].PutValue(50);
            
            // Créer une validation pour la cellule B7
            Validation validation = sheet.Cells["B7"].GetValidation();
            
            // Définir le type de validation et les formules
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "=B3";  // Demonstrating Formula2 usage
            
            // Appliquer la validation
            CellArea area = new CellArea();
            area.StartRow = 6;
            area.StartColumn = 1;
            area.EndRow = 6;
            area.EndColumn = 1;
            validation.AddArea(area);
            
            // Enregistrez le classeur
            workbook.Save("ValidationFormula2Demo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


