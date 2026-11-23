---
title: "ValidationCollection.RemoveArea"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ValidationCollection. Supprime tous les paramètres de validation sur la plage"
type: docs
url: /fr/net/aspose.cells/validationcollection/removearea/
---
## ValidationCollection.RemoveArea method

Supprime tous les paramètres de validation sur la plage.

```csharp
public void RemoveArea(CellArea ca)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ca | CellArea | La plage qui contient les paramètres de validation. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationCollectionMethodRemoveAreaDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer une validation dans une zone spécifique
            ValidationCollection validations = worksheet.Validations;
            CellArea validationArea = CellArea.CreateCellArea(0, 0, 5, 5);
            int validationIndex = validations.Add(validationArea);
            
            // Créer une zone à supprimer de la validation
            CellArea removeArea = CellArea.CreateCellArea(2, 2, 4, 4);
            
            try
            {
                // Appeler la méthode RemoveArea avec le paramètre CellArea
                validations.RemoveArea(removeArea);
                
                Console.WriteLine("Validation area removed successfully.");
                
                // Afficher les zones de validation restantes
                foreach (Validation validation in validations)
                {
                    if (validation.Areas.Length > 0)
                    {
                        Console.WriteLine($"Remaining validation area: {validation.Areas[0]}");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveArea method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("ValidationRemoveAreaDemo.xlsx");
        }
    }
}
```

### Voir aussi

* struct [CellArea](../../cellarea/)
* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


