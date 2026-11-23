---
title: "ValidationCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ValidationCollection. Obtient l'élément Validation à l'index spécifié"
type: docs
url: /fr/net/aspose.cells/validationcollection/item/
---
## ValidationCollection indexer

Obtient l'élément [`Validation`](../../validation/) à l'index spécifié.

```csharp
public Validation this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice à base zéro de l'élément. |

### Valeur de retour

L’élément à l’index spécifié.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter une validation de données aux cellules
            ValidationCollection validations = sheet.Validations;
            
            // Première zone de validation
            Validation validation1 = validations[validations.Add()];
            validation1.AddArea(new CellArea { StartRow = 1, StartColumn = 1, EndRow = 4, EndColumn = 3 });
            
            // Deuxième zone de validation
            Validation validation2 = validations[validations.Add()];
            validation2.AddArea(new CellArea { StartRow = 6, StartColumn = 1, EndRow = 6, EndColumn = 3 });

            // Accéder à la validation en utilisant la propriété Item
            Validation firstValidation = validations[0];
            Console.WriteLine($"First validation has {firstValidation.Areas.Length} area(s)");

            // Vérifier les zones
            foreach (CellArea area in firstValidation.Areas)
            {
                Console.WriteLine($"Area: {area.StartRow},{area.StartColumn} to {area.EndRow},{area.EndColumn}");
            }
        }
    }
}
```

### Voir aussi

* class [Validation](../../validation/)
* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


