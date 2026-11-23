---
title: "UnionRange.Merge"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode UnionRange. Combine une plage de cellules en une seule cellule"
type: docs
url: /fr/net/aspose.cells/unionrange/merge/
---
## UnionRange.Merge method

Combine une plage de cellules en une seule cellule.

```csharp
public void Merge()
```

### Remarques

Faites référence à la cellule fusionnée via l'adresse de la cellule en haut à gauche de la plage.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodMergeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer une plage de cellules (A1:B2)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "B2");
            
            // Insérer des données dans les cellules pour visualiser la fusion
            range[0, 0].PutValue("Before Merge");
            range[0, 1].PutValue("A1");
            range[1, 0].PutValue("B1");
            range[1, 1].PutValue("B2");
            
            try
            {
                // Créer un UnionRange à partir de la plage
                UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { range });
                
                // Appeler la méthode Merge
                unionRange.Merge();
                
                // Insérer une valeur dans la cellule fusionnée
                unionRange.PutValue("Merged A1:B2", true, true);
                
                Console.WriteLine("Cells merged successfully");
                
                // Décommentez pour voir l'effet de la défusion
                // unionRange.UnMerge();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Merge method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("MethodMergeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


