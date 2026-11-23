---
title: "Cells.GetRowOriginalHeightPoint"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Obtient la hauteur originale de la ligne en points si la ligne est masquée"
type: docs
url: /fr/net/aspose.cells/cells/getroworiginalheightpoint/
---
## Cells.GetRowOriginalHeightPoint method

Obtient la hauteur originale de la ligne en points si la ligne est masquée

```csharp
[Obsolete("Use Cells.GetRowHeight(int,bool,CellsUnitType) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double GetRowOriginalHeightPoint(int row)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | L'index de ligne. |

### Remarques

REMARQUE : ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode Cells.GetRowHeight(int,bool,CellsUnitType). Cette méthode sera supprimée 12 mois après avril 2024. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetRowOriginalHeightPointWithInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Enregistrer la hauteur originale avant modification
            double originalHeightBefore = cells.GetRowOriginalHeightPoint(0);
            
            // Modifier la hauteur de la ligne
            cells.SetRowHeight(0, 25.5);

            try
            {
                // Obtenir la hauteur originale après modification
                double originalHeight = cells.GetRowOriginalHeightPoint(0);
                double currentHeight = cells.GetRowHeight(0);

                Console.WriteLine($"Original row height: {originalHeight} points");
                Console.WriteLine($"Current row height: {currentHeight} points");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRowOriginalHeightPoint: {ex.Message}");
            }

            workbook.Save("GetRowOriginalHeightPointDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


