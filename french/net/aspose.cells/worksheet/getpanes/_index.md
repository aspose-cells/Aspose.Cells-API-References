---
title: "Worksheet.GetPanes"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Worksheet. Obtient les volets de la fenêtre"
type: docs
url: /fr/net/aspose.cells/worksheet/getpanes/
---
## Worksheet.GetPanes method

Obtient les volets de la fenêtre.

```csharp
public PaneCollection GetPanes()
```

### Remarques

Si la fenêtre n’est pas divisée ou figée.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodGetPanesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Figer les volets à la ligne 5 et à la colonne 3
            worksheet.FreezePanes(5, 3, 5, 3);
            
            // Obtenir les informations du volet
            PaneCollection panes = worksheet.GetPanes();
            
            // Afficher les informations du volet
            Console.WriteLine("First visible row of bottom pane: " + panes.FirstVisibleRowOfBottomPane);
            Console.WriteLine("First visible column of right pane: " + panes.FirstVisibleColumnOfRightPane);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [PaneCollection](../../panecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


