---
title: "DeleteBlankOptions.MergedCellsShrinkType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DeleteBlankOptions. Indique comment traiter les cellules fusionnées lors de la suppression de lignes/colonnes vides"
type: docs
url: /fr/net/aspose.cells/deleteblankoptions/mergedcellsshrinktype/
---
## DeleteBlankOptions.MergedCellsShrinkType property

Indique comment traiter les cellules fusionnées lors de la suppression des lignes/colonnes vides.

```csharp
public MergedCellsShrinkType MergedCellsShrinkType { get; set; }
```

### Remarques

Pour KeepHeaderOnly, toutes les cellules seront considérées comme vides sauf la cellule supérieure gauche non vide. C’est la valeur par défaut de cette propriété. Pour None, toutes les cellules seront considérées comme non vides. Pour ShrinkToFit, toutes les cellules en dehors de la zone d’affichage du contenu seront considérées comme vides.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyMergedCellsShrinkTypeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            Cells cells = ws.Cells;

            // Configurez des données d'exemple avec des cellules fusionnées
            cells.Merge(0, 0, 3, 1);
            cells[0, 0].PutValue("Merged Header");
            cells[3, 0].PutValue("Data after blank");
            
            // Créez des options de suppression avec différents types de réduction
            DeleteBlankOptions options = new DeleteBlankOptions();
            
            // Cas 1 : KeepHeaderOnly
            options.MergedCellsShrinkType = MergedCellsShrinkType.KeepHeaderOnly;
            cells.DeleteBlankRows(options);
            Console.WriteLine("After KeepHeaderOnly - Merged area preserved: " + 
                (cells.MergedCells.Count > 0 ? cells.MergedCells[0].ToString() : "No merged cells"));

            // Réinitialiser la feuille de calcul
            cells.ClearContents(0, 0, cells.MaxDataRow + 1, cells.MaxDataColumn + 1);
            cells.UnMerge(0, 0, 3, 1);
            cells.Merge(0, 0, 3, 1);
            cells[0, 0].PutValue("Merged Header");
            cells[3, 0].PutValue("Data after blank");

            // Cas 2 : ShrinkToFit
            options.MergedCellsShrinkType = MergedCellsShrinkType.ShrinkToFit;
            cells.DeleteBlankRows(options);
            Console.WriteLine("After ShrinkToFit - Merged area adjusted: " + 
                (cells.MergedCells.Count > 0 ? cells.MergedCells[0].ToString() : "No merged cells"));

            // Réinitialiser la feuille de calcul
            cells.ClearContents(0, 0, cells.MaxDataRow + 1, cells.MaxDataColumn + 1);
            cells.UnMerge(0, 0, 3, 1);
            cells.Merge(0, 0, 3, 1);
            cells[0, 0].PutValue("Merged Header");
            cells[3, 0].PutValue("Data after blank");

            // Cas 3 : None
            options.MergedCellsShrinkType = MergedCellsShrinkType.None;
            cells.DeleteBlankRows(options);
            Console.WriteLine("After None - Merged area unchanged: " + 
                (cells.MergedCells.Count > 0 ? cells.MergedCells[0].ToString() : "No merged cells"));
        }
    }
}
```

### Voir aussi

* enum [MergedCellsShrinkType](../../mergedcellsshrinktype/)
* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


