---
title: "ValidationCollection.RemoveACell"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ValidationCollection. Supprime tous les paramètres de validation de la cellule"
type: docs
url: /fr/net/aspose.cells/validationcollection/removeacell/
---
## ValidationCollection.RemoveACell method

Supprime tous les paramètres de validation sur la cellule.

```csharp
public void RemoveACell(int row, int column)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | L'index de ligne de la cellule. |
| column | Int32 | L'index de colonne de la cellule. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationCollectionMethodRemoveACellWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter une validation à la cellule A1 (ligne 0, colonne 0)
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            
            Validation validation = worksheet.Validations[worksheet.Validations.Add(area)];
            validation.Type = ValidationType.List;
            validation.Formula1 = "Item1,Item2,Item3";

            // Supprimer la validation de la cellule A1
            worksheet.Validations.RemoveACell(0, 0);

            Console.WriteLine("Validations count after removal: " + worksheet.Validations.Count);
        }
    }
}
```

### Voir aussi

* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


