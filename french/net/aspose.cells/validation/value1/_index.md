---
title: "Validation.Value1"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Validation. Représente la première valeur associée à la validation des données"
type: docs
url: /fr/net/aspose.cells/validation/value1/
---
## Validation.Value1 property

Représente la première valeur associée à la validation des données.

```csharp
public object Value1 { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyValue1Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une validation dans la cellule A1
            Validation validation = worksheet.Cells["A1"].GetValidation();
            validation.Type = ValidationType.List;
            
            // Définir la propriété Value1 avec un tableau de chaînes
            validation.Value1 = new object[] { "Option1", "Option2", "Option3" };

            // Obtenir et afficher les valeurs de validation
            object[] values = validation.Value1 as object[];
            Console.WriteLine("Validation values in A1:");
            foreach (object value in values)
            {
                Console.WriteLine(value.ToString());
            }

            // Créer une autre validation dans la cellule B1 avec des valeurs différentes
            Validation validation2 = worksheet.Cells["B1"].GetValidation();
            validation2.Type = ValidationType.List;
            validation2.Value1 = new object[] { "Yes", "No", "Maybe" };

            // Obtenir et afficher les valeurs de la deuxième validation
            object[] values2 = validation2.Value1 as object[];
            Console.WriteLine("\nValidation values in B1:");
            foreach (object value in values2)
            {
                Console.WriteLine(value.ToString());
            }
        }
    }
}
```

### Voir aussi

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


