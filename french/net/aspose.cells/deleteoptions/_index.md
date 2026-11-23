---
title: "Classe DeleteOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.DeleteOptions. Représente le paramètre de suppression des lignes/colonnes"
type: docs
url: /fr/net/aspose.cells/deleteoptions/
---
## DeleteOptions class

Représente le paramètre de suppression des lignes/colonnes.

```csharp
public class DeleteOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [DeleteOptions](deleteoptions/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [FormulaChangeMonitor](../../aspose.cells/deleteoptions/formulachangemonitor/) { get; set; } | Obtient/définit le moniteur pour suivre les modifications causées par la suppression. |
| [UpdateReference](../../aspose.cells/deleteoptions/updatereference/) { get; set; } | Indique si les références sont mises à jour dans d'autres feuilles de calcul. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DeleteOptionsDemo
    {
        public static void DeleteOptionsExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter des données à la feuille de calcul
            sheet.Cells["A1"].PutValue("Item");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["A4"].PutValue("Cherry");

            // Afficher les données d'origine
            Console.WriteLine("Original Data:");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(sheet.Cells[$"A{i}"].Value);
            }

            // Créer DeleteOptions
            DeleteOptions options = new DeleteOptions
            {
                UpdateReference = true // Set to true to update references in other worksheets
            };

            // Supprimer la deuxième ligne (Banana)
            sheet.Cells.DeleteRow(2, options.UpdateReference);

            // Afficher les données après la suppression
            Console.WriteLine("\nData After Deletion:");
            for (int i = 1; i <= 3; i++)
            {
                Console.WriteLine(sheet.Cells[$"A{i}"].Value);
            }

            // Enregistrez le classeur
            workbook.Save("DeleteOptionsExample.xlsx");
            workbook.Save("DeleteOptionsExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


