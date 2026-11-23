---
title: "Validation.InCellDropDown"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Validation. Indique si la validation des données affiche une liste déroulante contenant des valeurs acceptables"
type: docs
url: /fr/net/aspose.cells/validation/incelldropdown/
---
## Validation.InCellDropDown property

Indique si la validation des données affiche une liste déroulante contenant des valeurs acceptables.

```csharp
public bool InCellDropDown { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyInCellDropDownDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une validation pour la cellule A1
            Validation validation = worksheet.Cells["A1"].GetValidation();
            
            // Définir le type de validation sur une liste avec des valeurs
            validation.Type = ValidationType.List;
            validation.Formula1 = "Option1,Option2,Option3";
            
            // Activer la liste déroulante en cellule
            validation.InCellDropDown = true;

            // Créer une autre validation pour la cellule B1 sans liste déroulante
            Validation validation2 = worksheet.Cells["B1"].GetValidation();
            validation2.Type = ValidationType.List;
            validation2.Formula1 = "Choice1,Choice2,Choice3";
            validation2.InCellDropDown = false;

            // Enregistrez le classeur
            workbook.Save("InCellDropDownDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


