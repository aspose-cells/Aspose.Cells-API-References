---
title: "PaneCollection.AcitvePaneType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PaneCollection. Obtient et définit le volet actif"
type: docs
url: /fr/net/aspose.cells/panecollection/acitvepanetype/
---
## PaneCollection.AcitvePaneType property

Obtient et définit le volet actif.

```csharp
[Obsolete("Use PaneCollection.ActivePaneType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public RectangleAlignmentType AcitvePaneType { get; set; }
```

### Remarques

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété [`ActivePaneType`](../activepanetype/). Cette méthode sera supprimée 12 mois plus tard à compter de juillet 2026. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class PaneCollectionPropertyAcitvePaneTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour démontrer le fractionnement des volets
            for (int i = 0; i < 20; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].Value = $"Row {i + 1}, Col {j + 1}";
                }
            }

            // Diviser la feuille de calcul en volets
            worksheet.Split();

            // Obtenir la collection de volets
            PaneCollection panes = worksheet.GetPanes();

            // Afficher le volet actif actuel
            Console.WriteLine("Current ActivePaneType: " + panes.AcitvePaneType);

            // Définir le volet actif sur BottomRight
            panes.AcitvePaneType = RectangleAlignmentType.BottomRight;
            Console.WriteLine("Changed ActivePaneType to: " + panes.AcitvePaneType);

            // Définir la première ligne/colonne visible pour les volets inférieur/droit
            panes.FirstVisibleRowOfBottomPane = 15;
            panes.FirstVisibleColumnOfRightPane = 7;

            // Enregistrez le classeur
            workbook.Save("PaneCollectionActivePaneTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [RectangleAlignmentType](../../../aspose.cells.drawing/rectanglealignmenttype/)
* class [PaneCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


