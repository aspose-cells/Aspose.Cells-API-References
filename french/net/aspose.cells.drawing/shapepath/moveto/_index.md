---
title: "ShapePath.MoveTo"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapePath. Commence une nouvelle figure à partir du point spécifié sans fermer la figure actuelle. Tous les points suivants ajoutés au chemin sont ajoutés à cette nouvelle figure. Unité Pixel"
type: docs
url: /fr/net/aspose.cells.drawing/shapepath/moveto/
---
## ShapePath.MoveTo method

Démarre une nouvelle figure à partir du point spécifié sans fermer la figure actuelle. Tous les points suivants ajoutés au chemin sont ajoutés à cette nouvelle figure. Unité : Pixel.

```csharp
public void MoveTo(float x, float y)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| x | Single | La coordonnée x du point de départ de la figure (Unité : Pixel). |
| y | Single | La coordonnée y du point de départ de la figure (Unité : Pixel). |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodMoveToWithSingleSingleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                //Créer un nouveau chemin de forme
                ShapePath shapePath = new ShapePath();

                // Déplacer vers le point de départ
                shapePath.MoveTo(10, 10);

                // Appeler la méthode LineTo avec les paramètres (Single, Single)
                shapePath.LineTo(50.5f, 10.5f);
                shapePath.LineTo(50.5f, 50.5f);
                shapePath.LineTo(10.5f, 50.5f);
                shapePath.Close();

                //ajouter une forme libre
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath });

                Console.WriteLine("MoveTo method executed successfully with parameters (Single, Single)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing LineTo method: {ex.Message}");
            }
           
            
            // Enregistrer le résultat
            workbook.Save("ShapePathMethodMoveToWithSingleSingleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


