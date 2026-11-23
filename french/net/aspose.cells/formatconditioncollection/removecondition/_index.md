---
title: "FormatConditionCollection.RemoveCondition"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode FormatConditionCollection. Supprime la condition de formatage par indice"
type: docs
url: /fr/net/aspose.cells/formatconditioncollection/removecondition/
---
## FormatConditionCollection.RemoveCondition method

Supprime la condition de formatage par index.

```csharp
public void RemoveCondition(int index)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indice | Int32 | L'indice de la condition de formatage à supprimer. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormatConditionCollectionMethodRemoveConditionWithInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtenir la collection des conditions de formatage
            FormatConditionCollection formatConditions = worksheet.ConditionalFormattings[0];
            
            // Ajouter quelques conditions d'exemple
            int index1 = formatConditions.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");
            int index2 = formatConditions.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "50", "");
            
            try
            {
                // Afficher le nombre initial
                Console.WriteLine($"Initial conditions count: {formatConditions.Count}");
                
                // Supprimer la première condition
                formatConditions.RemoveCondition(index1);
                
                // Afficher le nombre mis à jour
                Console.WriteLine($"Conditions count after removal: {formatConditions.Count}");
                
                // Enregistrez le classeur
                workbook.Save("RemoveConditionDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling RemoveCondition: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


