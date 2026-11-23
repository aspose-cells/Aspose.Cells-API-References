---
title: "Cells.GetViewRowHeightInch"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Obtient la hauteur d’une ligne spécifiée en unités de pouces"
type: docs
url: /fr/net/aspose.cells/cells/getviewrowheightinch/
---
## Cells.GetViewRowHeightInch method

Obtient la hauteur d'une ligne spécifiée en pouces.

```csharp
public double GetViewRowHeightInch(int row)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | Indice de ligne |

### Valeur de retour

Hauteur de la ligne

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetViewRowHeightInchWithInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir une hauteur de ligne personnalisée pour la ligne 2 en pouces
            worksheet.Cells.SetRowHeightInch(2, 1.5);

            try
            {
                // Appeler GetViewRowHeightInch avec le paramètre d'index de ligne
                double rowHeight = worksheet.Cells.GetViewRowHeightInch(2);
                
                // Afficher le résultat et vérifier que la hauteur correspond à la valeur définie
                Console.WriteLine($"View row height of row 2: {rowHeight} inches");
                
                // Démontrer l'effet en ajoutant du contenu d'exemple
                worksheet.Cells["A2"].PutValue($"Row Height: {rowHeight}\"");
                worksheet.Cells.SetColumnWidthInch(0, 15);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetViewRowHeightInch: {ex.Message}");
            }
            
            // Enregistrer le classeur modifié
            workbook.Save("CellsMethodGetViewRowHeightInchWithInt32Demo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


