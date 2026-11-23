---
title: "PictureCollection.Camera"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PictureCollection. Prend une photo de la plage"
type: docs
url: /fr/net/aspose.cells.drawing/picturecollection/camera/
---
## PictureCollection.Camera method

Prend une photo de la plage.

```csharp
public int Camera(int row, int column, string range)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | L'indice de ligne de cette image. |
| column | Int32 | L'indice de colonne de cette image. |
| plage | String | La zone qui nécessite une photographie |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class PictureCollectionMethodCameraWithInt32Int32StringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple pour créer une plage
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "More Data";
            worksheet.Cells["A2"].Value = "Row 2";
            worksheet.Cells["B2"].Value = "Row 2 Col 2";

            try
            {
                // Obtenez la collection Pictures de la feuille de calcul
                PictureCollection pictures = worksheet.Pictures;

                // Appelez la méthode Camera pour créer une image de caméra
                // Paramètres : row (top-left row), column (top-left column), range (source range)
                int pictureIndex = pictures.Camera(5, 1, "A1:B2");

                Console.WriteLine($"Camera picture added successfully at index: {pictureIndex}");

                // Enregistrez le classeur
                workbook.Save("CameraDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling Camera method: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


