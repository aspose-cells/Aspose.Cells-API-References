---
title: "Cells.GetMaxGroupedRowOutlineLevel"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Obtient le niveau de contour de ligne groupée maximal basé sur zéro"
type: docs
url: /fr/net/aspose.cells/cells/getmaxgroupedrowoutlinelevel/
---
## Cells.GetMaxGroupedRowOutlineLevel method

Obtient le niveau de contour maximal des lignes groupées (à base zéro).

```csharp
public int GetMaxGroupedRowOutlineLevel()
```

### Valeur de retour

Le niveau de contour de ligne groupée maximal (à base zéro)

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetMaxGroupedRowOutlineLevelDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Regroupez certaines lignes pour démontrer les niveaux de contour
            cells.GroupRows(0, 2, false);
            cells.GroupRows(4, 6, false);
            
            // Ajoutez un groupement imbriqué
            cells.GroupRows(4, 5, true);

            // Obtenez le niveau de contour de ligne groupée maximal
            int maxOutlineLevel = cells.GetMaxGroupedRowOutlineLevel();

            // Afficher le résultat
            Console.WriteLine("Maximum grouped row outline level: " + maxOutlineLevel);

            // Affichez le niveau de contour pour chaque ligne
            for (int row = 0; row <= 6; row++)
            {
                Console.WriteLine($"Row {row} outline level: {cells.GetGroupedRowOutlineLevel(row)}");
            }
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


