---
title: "ShapePath.Close"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapePath. Ferme la figure actuelle et commence une nouvelle figure. Si la figure actuelle contient une séquence de lignes et de courbes connectées, la méthode ferme la boucle en reliant une ligne du point final au point de départ."
type: docs
url: /fr/net/aspose.cells.drawing/shapepath/close/
---
## ShapePath.Close method

Ferme la figure actuelle et démarre une nouvelle figure. Si la figure actuelle contient une séquence de lignes et de courbes connectées, la méthode ferme la boucle en reliant une ligne du point final au point de départ.

```csharp
public void Close()
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodCloseDemo
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
                shapePath.MoveTo(60, 45);
                shapePath.ArcTo(25, 25, 0, 270);

                // Fermer le chemin
                shapePath.Close();

                shapePath.MoveTo(60, 20);
                shapePath.LineTo(110, 70);
                shapePath.LineTo(125, 155.5f);
                shapePath.ArcTo(35.5f, 35.5f, 0, 270);

                // Fermer le chemin
                shapePath.Close();

                //ajouter une forme libre
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath });

                Console.WriteLine("Close method called successfully to complete the shape path");
                
                // Enregistrez le classeur
                workbook.Save("ShapePathMethodCloseDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling Close method: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


