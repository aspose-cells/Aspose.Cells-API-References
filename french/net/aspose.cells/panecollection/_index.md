---
title: "Classe PaneCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.PaneCollection class. Représente tous les objets Pane affichés dans la fenêtre spécifiée"
type: docs
url: /fr/net/aspose.cells/panecollection/
---
## PaneCollection class

Représente tous les objets Pane affichés dans la fenêtre spécifiée.

```csharp
public class PaneCollection
```

## Propriétés

| Nom | Description |
| --- | --- |
| [AcitvePaneType](../../aspose.cells/panecollection/acitvepanetype/) { get; set; } | (**Obsolete.**) Obtient et définit le volet actif. |
| [ActivePaneType](../../aspose.cells/panecollection/activepanetype/) { get; set; } | Obtient et définit le volet actif. |
| [FirstVisibleColumnOfRightPane](../../aspose.cells/panecollection/firstvisiblecolumnofrightpane/) { get; set; } | Obtient et définit la première colonne visible du volet droit. |
| [FirstVisibleRowOfBottomPane](../../aspose.cells/panecollection/firstvisiblerowofbottompane/) { get; set; } | Obtient et définit la première ligne visible du volet inférieur. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassPaneCollectionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    sheet.Cells[i, j].Value = $"Row {i}, Col {j}";
                }
            }
            
            // Figer les volets à la ligne 5, colonne 1
            sheet.FreezePanes(5, 1, 5, 1);
            
            // Obtenir la collection de volets
            PaneCollection panes = sheet.GetPanes();
            
            // Modifier les paramètres du volet
            panes.FirstVisibleRowOfBottomPane = 5;
            panes.FirstVisibleColumnOfRightPane = 1;
            
            // Enregistrez le classeur
            workbook.Save("PaneCollectionDemo.xls", SaveFormat.Excel97To2003);
            
            Console.WriteLine("PaneCollection demo executed successfully.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


