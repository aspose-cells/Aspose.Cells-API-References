---
title: "Cells.GetCellsWithPlaceInCellPicture"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Obtient toutes les cellules qui contiennent une image intégrée"
type: docs
url: /fr/net/aspose.cells/cells/getcellswithplaceincellpicture/
---
## Cells.GetCellsWithPlaceInCellPicture method

Obtient toutes les cellules qui contiennent une image intégrée.

```csharp
public IEnumerator GetCellsWithPlaceInCellPicture()
```

### Valeur de retour

Énumérateur pour parcourir tous les objets Cell qui contiennent une image intégrée

### Remarques

S'il n'y a aucune image définie comme "Place in Cell" dans cette feuille de calcul, null sera retourné.

### Exemples

```csharp
using System;
using System.IO;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetCellsWithPlaceInCellPictureDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une image à la feuille de calcul (cela ne sera pas compté par GetCellsWithPlaceInCellPicture)
            workbook.Worksheets[0].Pictures.Add(0, 0, "sample.png");
            
            // Ajouter une image intégrée à la cellule B3 (cela sera compté)
            workbook.Worksheets[0].Cells["B3"].EmbeddedImage = File.ReadAllBytes("sample.png");
            
            // Supprimer l'image flottante
            workbook.Worksheets[0].Pictures.RemoveAt(0);

            // Obtenir les cellules avec des images intégrées
            Cells cells = workbook.Worksheets[0].Cells;
            int count = 0;
            
            IEnumerator enumerator = cells.GetCellsWithPlaceInCellPicture();
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                byte[] imageData = cell.EmbeddedImage;
                if (imageData != null)
                {
                    count++;
                    Console.WriteLine($"Found image in cell {cell.Name}");
                }
            }
            
            Console.WriteLine($"Total cells with embedded images: {count}");
            
            // Enregistrer et recharger pour vérifier la persistance
            workbook.Save("output.xlsx");
            workbook = new Workbook("output.xlsx");
            
            // Vérifier après rechargement
            cells = workbook.Worksheets[0].Cells;
            count = 0;
            enumerator = cells.GetCellsWithPlaceInCellPicture();
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                byte[] imageData = cell.EmbeddedImage;
                if (imageData != null)
                {
                    count++;
                }
            }
            Console.WriteLine($"After reload - cells with embedded images: {count}");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


