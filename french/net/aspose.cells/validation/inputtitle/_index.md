---
title: "Validation.InputTitle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Validation. Représente le titre de la boîte de dialogue d’entrée de validation de données"
type: docs
url: /fr/net/aspose.cells/validation/inputtitle/
---
## Validation.InputTitle property

Représente le titre de la boîte de dialogue d'entrée de validation des données.

```csharp
public string InputTitle { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyInputTitleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer un objet de validation
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.IgnoreBlank = true;
            
            // Définir la plage de validation
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 0;
            area.StartColumn = 0;
            area.EndColumn = 0;
            validation.AddArea(area);

            // Définir les propriétés de validation
            validation.Formula1 = "10";
            validation.Formula2 = "100";
            validation.Operator = OperatorType.Between;
            
            // Définir les propriétés du message d'entrée
            validation.InputTitle = "Number Validation";
            validation.InputMessage = "Please enter a number between 10 and 100";
            
            // Enregistrez le classeur
            workbook.Save("ValidationInputTitleDemo.xlsx");
            
            // Vérifier la propriété InputTitle
            Console.WriteLine("Validation InputTitle: " + validation.InputTitle);
        }
    }
}
```

### Voir aussi

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


