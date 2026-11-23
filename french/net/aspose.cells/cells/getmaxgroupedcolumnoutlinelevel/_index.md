---
title: "Cells.GetMaxGroupedColumnOutlineLevel"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Obtient le niveau de contour de colonne groupée maximal, indexé à zéro"
type: docs
url: /fr/net/aspose.cells/cells/getmaxgroupedcolumnoutlinelevel/
---
## Cells.GetMaxGroupedColumnOutlineLevel method

Obtient le niveau de contour maximal des colonnes groupées (à base zéro).

```csharp
public int GetMaxGroupedColumnOutlineLevel()
```

### Valeur de retour

Le niveau de contour de colonne groupée maximal (indexé à zéro)

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetMaxGroupedColumnOutlineLevelDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Regrouper certaines colonnes pour démontrer les niveaux de contour
            cells.GroupColumns(0, 2, false);
            cells.GroupColumns(3, 5, false);
            
            // Obtenir le niveau de contour de colonne groupée maximal
            int maxOutlineLevel = cells.GetMaxGroupedColumnOutlineLevel();
            
            Console.WriteLine("Maximum grouped column outline level: " + maxOutlineLevel);
            
            // Afficher le niveau de contour pour chaque colonne
            for (int col = 0; col < 6; col++)
            {
                int outlineLevel = cells.GetGroupedColumnOutlineLevel(col);
                Console.WriteLine($"Column {col} outline level: {outlineLevel}");
            }
            
            // Enregistrez le classeur
            workbook.Save("GroupedColumnsOutlineLevel.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


