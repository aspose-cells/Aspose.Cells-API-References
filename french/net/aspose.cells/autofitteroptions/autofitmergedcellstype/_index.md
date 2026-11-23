---
title: "AutoFitterOptions.AutoFitMergedCellsType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété AutoFitterOptions. Obtient et définit le type d'ajustement automatique de la hauteur des lignes des cellules fusionnées"
type: docs
url: /fr/net/aspose.cells/autofitteroptions/autofitmergedcellstype/
---
## AutoFitterOptions.AutoFitMergedCellsType property

Obtient et définit le type d'ajustement automatique de la hauteur de ligne des cellules fusionnées.

```csharp
public AutoFitMergedCellsType AutoFitMergedCellsType { get; set; }
```

### Remarques

Excel ignore par défaut les cellules fusionnées lors de l'ajustement de la hauteur des lignes, ainsi Aspose.Cells fonctionne comme le comportement par défaut de MS Excel. Veuillez définir ce type pour modifier la façon d'ajuster automatiquement la hauteur des lignes des cellules fusionnées.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyAutoFitMergedCellsTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir des données d'exemple et fusionner les cellules
            worksheet.Cells["A1"].PutValue("This is a sample text for merged cells auto-fit demonstration");
            worksheet.Cells.Merge(0, 0, 3, 2); // Merge A1:B3

            // Ajuster automatiquement les lignes avec AutoFitMergedCellsType.EachLine
            worksheet.AutoFitRows(new AutoFitterOptions
            {
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph
            });

            // Ajuster automatiquement les colonnes avec AutoFitMergedCellsType.EachLine
            worksheet.AutoFitColumns(new AutoFitterOptions
            {
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph
            });

            // Enregistrez le classeur
            workbook.Save("AutoFitMergedCellsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [AutoFitMergedCellsType](../../autofitmergedcellstype/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


