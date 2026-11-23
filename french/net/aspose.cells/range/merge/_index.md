---
title: "Range.Merge"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Range. Combine une plage de cellules en une seule cellule"
type: docs
url: /fr/net/aspose.cells/range/merge/
---
## Range.Merge method

Combine une plage de cellules en une seule cellule.

```csharp
public void Merge()
```

### Remarques

Faites référence à la cellule fusionnée via l'adresse de la cellule en haut à gauche de la plage.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodMergeDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une plage et fusionner les cellules (3 lignes x 2 colonnes)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 3, 2);
            range.Merge();

            // Définir la valeur dans la cellule fusionnée
            worksheet.Cells[0, 0].Value = "Merged Cells Demo";

            // Appliquer un style aux cellules fusionnées
            Style style = worksheet.Cells[0, 0].GetStyle();
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.Font.IsBold = true;
            worksheet.Cells[0, 0].SetStyle(style);

            // Enregistrez le classeur
            workbook.Save("MergedCellsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


