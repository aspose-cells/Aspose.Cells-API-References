---
title: "Cells.MergedCells"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cells. Obtient la collection de cellules fusionnées"
type: docs
url: /fr/net/aspose.cells/cells/mergedcells/
---
## Cells.MergedCells property

Obtient la collection de cellules fusionnées.

```csharp
[Obsolete("Use Cells.GetMergedAreas() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList MergedCells { get; }
```

### Remarques

Dans cette collection, chaque élément est une structure [`CellArea`](../../cellarea/) qui représente une zone de cellules fusionnées.

NOTE: Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode Cells.GetMergedAreas(). Cette méthode sera supprimée 12 mois plus tard, depuis novembre 2023. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellsPropertyMergedCellsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Fusionner des cellules dans deux plages différentes
            cells.Merge(0, 0, 2, 2); // Merges A1:B2
            cells.Merge(2, 2, 2, 2); // Merges C3:D4

            // Accéder à la propriété MergedCells (lecture seule)
            ArrayList mergedRanges = cells.MergedCells;

            // Afficher le nombre initial de cellules fusionnées et les plages
            Console.WriteLine($"Initial merged cells count: {mergedRanges.Count}");
            foreach (CellArea area in mergedRanges)
            {
                Console.WriteLine($"Merged area: Row[{area.StartRow}-{area.EndRow}], Column[{area.StartColumn}-{area.EndColumn}]");
            }

            // Annuler la fusion de la première plage fusionnée
            cells.UnMerge(0, 0, 2, 2);

            // Afficher le nombre mis à jour de cellules fusionnées et les plages
            Console.WriteLine($"\nAfter unmerging A1:B2 - Merged cells count: {cells.MergedCells.Count}");
            foreach (CellArea area in cells.MergedCells)
            {
                Console.WriteLine($"Remaining merged area: Row[{area.StartRow}-{area.EndRow}], Column[{area.StartColumn}-{area.EndColumn}]");
            }

            // Enregistrer le résultat
            workbook.Save("PropertyMergedCellsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


