---
title: "Validation.InputMessage"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Validation. Représente le message d'entrée de la validation des données"
type: docs
url: /fr/net/aspose.cells/validation/inputmessage/
---
## Validation.InputMessage property

Représente le message d'entrée de validation des données.

```csharp
public string InputMessage { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyInputMessageDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une validation
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.List;
            validation.Formula1 = "Yes,No";
            validation.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });
            validation.IgnoreBlank = true;
            validation.InCellDropDown = true;
            
            // Définir les propriétés du message d'entrée
            validation.ShowInput = true;
            validation.InputTitle = "Selection Required";
            validation.InputMessage = "Please select either Yes or No from the dropdown";

            // Enregistrez le classeur
            workbook.Save("ValidationInputMessageDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


