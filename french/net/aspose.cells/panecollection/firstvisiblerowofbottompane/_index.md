---
title: "PaneCollection.FirstVisibleRowOfBottomPane"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PaneCollection. Obtient et définit la première ligne visible du volet inférieur"
type: docs
url: /fr/net/aspose.cells/panecollection/firstvisiblerowofbottompane/
---
## PaneCollection.FirstVisibleRowOfBottomPane property

Obtient et définit la première ligne visible du volet inférieur.

```csharp
public int FirstVisibleRowOfBottomPane { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaneCollectionPropertyFirstVisibleRowOfBottomPaneDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour créer un volet défilable
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }
            
            // Figer les volets à la ligne 10 (cela créera des volets supérieur et inférieur)
            worksheet.FreezePanes(10, 0, 10, 0);
            
            // Obtenir la collection de volets
            PaneCollection panes = worksheet.GetPanes();
            
            // Définir la première ligne visible du volet inférieur
            panes.FirstVisibleRowOfBottomPane = 15;
            
            // Afficher la première ligne visible du volet inférieur
            Console.WriteLine("First visible row of bottom pane: " + panes.FirstVisibleRowOfBottomPane);
            
            // Enregistrez le classeur
            workbook.Save("PaneCollectionPropertyFirstVisibleRowOfBottomPaneDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PaneCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


