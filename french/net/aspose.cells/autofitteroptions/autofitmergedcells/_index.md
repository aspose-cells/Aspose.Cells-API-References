---
title: "AutoFitterOptions.AutoFitMergedCells"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété AutoFitterOptions. Indique si la hauteur de ligne doit être ajustée automatiquement lorsque les cellules sont fusionnées dans une ligne. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells/autofitteroptions/autofitmergedcells/
---
## AutoFitterOptions.AutoFitMergedCells property

Indique si la hauteur de ligne doit être ajustée automatiquement lorsque les cellules sont fusionnées dans une ligne. La valeur par défaut est false.

```csharp
[Obsolete("Use AutoFitterOptions.AutoFitMergedCellsType property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool AutoFitMergedCells { get; set; }
```

### Remarques

REMARQUE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la propriété AutoFitterOptions.AutoFitMergedCellsType. Cette propriété sera supprimée 12 mois plus tard, à compter de décembre 2018. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyAutoFitMergedCellsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer des données d'exemple et fusionner les cellules
            worksheet.Cells["A1"].PutValue("This is a test of AutoFitMergedCells property");
            worksheet.Cells.Merge(0, 0, 3, 3); // Merge cells A1:C3

            // Créer AutoFitterOptions et définir AutoFitMergedCells
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitMergedCells = true;

            // Ajuster automatiquement les lignes avec des cellules fusionnées
            worksheet.AutoFitRows(options);

            // Enregistrez le classeur
            workbook.Save("AutoFitMergedCellsExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


