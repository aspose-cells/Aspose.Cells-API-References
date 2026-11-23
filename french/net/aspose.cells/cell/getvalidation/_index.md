---
title: "Cell.GetValidation"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cell. Obtient la validation appliquée à cette cellule"
type: docs
url: /fr/net/aspose.cells/cell/getvalidation/
---
## Cell.GetValidation method

Obtient la validation appliquée à cette cellule.

```csharp
public Validation GetValidation()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetValidationDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accéder à la cellule B5 et ajouter une validation
            Cell cell = worksheet.Cells["B5"];
            Validation validation = cell.GetValidation();
            
            // Définir le type de validation et afficher le message
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "20";
            validation.ShowError = true;
            validation.ErrorMessage = "Enter value between 10 and 20";
            
            // Enregistrez le classeur
            workbook.Save("ValidationDemo.xlsx");
            
            // Vérifier la validation
            Validation retrievedValidation = cell.GetValidation();
            Console.WriteLine("Validation Type: " + retrievedValidation.Type);
            Console.WriteLine("Validation Message: " + retrievedValidation.ErrorMessage);
        }
    }
}
```

### Voir aussi

* class [Validation](../../validation/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


