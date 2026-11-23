---
title: "ConditionalFormattingCollection.RemoveArea"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ConditionalFormattingCollection. Supprimez toute la mise en forme conditionnelle dans la plage"
type: docs
url: /fr/net/aspose.cells/conditionalformattingcollection/removearea/
---
## ConditionalFormattingCollection.RemoveArea method

Supprime tout le formatage conditionnel dans la plage.

```csharp
public void RemoveArea(int startRow, int startColumn, int totalRows, int totalColumns)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | Int32 | La ligne de départ de la plage. |
| startColumn | Int32 | La colonne de départ de la plage. |
| totalRows | Int32 | Le nombre de lignes de la plage. |
| totalColumns | Int32 | Le nombre de colonnes de la plage. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingCollectionMethodRemoveAreaWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtenez la collection de mise en forme conditionnelle
            ConditionalFormattingCollection cfc = worksheet.ConditionalFormattings;

            // Ajoutez quelques règles de mise en forme conditionnelle
            int index = cfc.Add();
            FormatConditionCollection fcc = cfc[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 5;
            area.EndColumn = 5;
            fcc.AddArea(area);

            try
            {
                // Appelez RemoveArea avec les paramètres (Int32, Int32, Int32, Int32)
                cfc.RemoveArea(0, 0, 3, 3);

                Console.WriteLine("Conditional formatting removed from area (0,0,3,3)");
                
                // Vérifiez l'effet en vérifiant le compteur (cela serait 0 si toute la mise en forme a été supprimée)
                Console.WriteLine($"Remaining conditional formatting areas: {fcc.RangeCount}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveArea method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("RemoveAreaWithInt32Demo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ConditionalFormattingCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


