---
title: "Validation.ShowInput"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Validation. Indique si le message d'entrée de validation des données sera affiché chaque fois que l'utilisateur sélectionne une cellule dans la plage de validation des données"
type: docs
url: /fr/net/aspose.cells/validation/showinput/
---
## Validation.ShowInput property

Indique si le message d'entrée de validation des données sera affiché chaque fois que l'utilisateur sélectionne une cellule dans la plage de validation des données.

```csharp
public bool ShowInput { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyShowInputDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une zone de validation
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 0;
            area.StartColumn = 0;
            area.EndColumn = 0;

            // Ajouter une validation
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.List;
            validation.Formula1 = "Yes,No";
            validation.IgnoreBlank = true;
            validation.InCellDropDown = true;
            
            // Définir la propriété ShowInput
            validation.ShowInput = true;
            validation.InputTitle = "Selection";
            validation.InputMessage = "Please select Yes or No";

            validation.AddArea(area);

            // Enregistrez le classeur
            workbook.Save("ValidationPropertyShowInputDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


