---
title: "Classe DeleteBlankOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.DeleteBlankOptions classe. Représente le paramètre de suppression des cellules/ lignes/colonnes vides"
type: docs
url: /fr/net/aspose.cells/deleteblankoptions/
---
## DeleteBlankOptions class

Représente le paramètre de suppression des cellules/lignes/colonnes vides.

```csharp
public class DeleteBlankOptions : DeleteOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [DeleteBlankOptions](deleteblankoptions/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [DrawingsAsBlank](../../aspose.cells/deleteblankoptions/drawingsasblank/) { get; set; } | Indique si les objets liés au dessin tels que l'image, la forme, le graphique... seront considérés comme vides. La valeur par défaut est true. |
| [EmptyFormulaValueAsBlank](../../aspose.cells/deleteblankoptions/emptyformulavalueasblank/) { get; set; } | Indique si une cellule sera considérée comme vide lorsqu'elle est une formule et que le résultat calculé est nul ou une chaîne vide. La valeur par défaut est false. |
| [EmptyStringAsBlank](../../aspose.cells/deleteblankoptions/emptystringasblank/) { get; set; } | Indique si une cellule sera considérée comme vide lorsque sa valeur est une chaîne vide. La valeur par défaut est true. |
| [EndIndex](../../aspose.cells/deleteblankoptions/endindex/) { get; set; } | Spécifie l'index de fin de ligne/colonne (inclusif) de la plage à vérifier et à supprimer les lignes/colonnes vides. La valeur par défaut est -1 et -1 signifie la plage maximale de tous les objets (cellules, dessins, ...) qui doivent être vérifiés. |
| [FormulaChangeMonitor](../../aspose.cells/deleteoptions/formulachangemonitor/) { get; set; } | Obtient/definit le moniteur pour suivre les modifications causées par la suppression.(Hérité de [`DeleteOptions`](../deleteoptions/).) |
| [MergedCellsShrinkType](../../aspose.cells/deleteblankoptions/mergedcellsshrinktype/) { get; set; } | Indique comment traiter les cellules fusionnées lors de la suppression des lignes/colonnes vides. |
| [StartIndex](../../aspose.cells/deleteblankoptions/startindex/) { get; set; } | Spécifie l'index de début de ligne/colonne de la plage à vérifier et à supprimer les lignes/colonnes vides. |
| [UpdateReference](../../aspose.cells/deleteoptions/updatereference/) { get; set; } | Indique si mettre à jour les références dans d'autres feuilles de calcul.(Hérité de [`DeleteOptions`](../deleteoptions/).) |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DeleteBlankOptionsDemo
    {
        public static void DeleteBlankOptionsExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplissez la feuille de calcul avec quelques données
            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue("");
            worksheet.Cells["A3"].PutValue("More Data");
            worksheet.Cells["A4"].PutValue("");
            worksheet.Cells["A5"].PutValue("Even More Data");

            // Créez une instance de DeleteBlankOptions
            DeleteBlankOptions options = new DeleteBlankOptions
            {
                EmptyStringAsBlank = true,
                EmptyFormulaValueAsBlank = false,
                UpdateReference = true
            };

            // Supprimez les lignes vides en fonction des options
            worksheet.Cells.DeleteBlankRows(options);

            // Enregistrez le classeur
            workbook.Save("DeleteBlankOptionsExample.xlsx");
            workbook.Save("DeleteBlankOptionsExample.pdf");
            return;
        }
    }
}
```

### Voir aussi

* class [DeleteOptions](../deleteoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


