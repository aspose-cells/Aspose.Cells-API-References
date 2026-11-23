---
title: "Validation.RemoveACell"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode de validation. Supprimez les paramètres de validation dans la cellule"
type: docs
url: /fr/net/aspose.cells/validation/removeacell/
---
## Validation.RemoveACell method

Supprime les paramètres de validation dans la cellule.

```csharp
public void RemoveACell(int row, int column)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | L'index de ligne. |
| column | Int32 | L'index de colonne. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodRemoveACellWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez une validation de données à la première cellule
            Validation validation = worksheet.Validations[0];
            validation.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });
            validation.Type = ValidationType.List;
            validation.Formula1 = "1,2,3";
            
            // Ajoutez une autre cellule à la validation
            validation.AddArea(new CellArea { StartRow = 1, StartColumn = 1, EndRow = 1, EndColumn = 1 });
            
            // Supprimez la deuxième cellule de la validation
            validation.RemoveACell(1, 1);
            
            Console.WriteLine("Cell removed from validation successfully.");
        }
    }
}
```

### Voir aussi

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


