---
title: "ShapeCollection.AddPictureInChart"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapeCollection. Ajoute une image au graphique"
type: docs
url: /fr/net/aspose.cells.drawing/shapecollection/addpictureinchart/
---
## ShapeCollection.AddPictureInChart method

Ajoute une image au graphique.

```csharp
public Picture AddPictureInChart(int top, int left, Stream stream, int widthScale, int heightScale)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| haut | Int32 | Représente le décalage vertical de la forme depuis le coin supérieur gauche en unités de 1/4000 de la zone du graphique. |
| gauche | Int32 | Représente le décalage horizontal de la forme par rapport au coin supérieur gauche en unités de 1/4000 de la zone du graphique. |
| stream | Stream | Objet Stream qui contient les données de l'image. |
| widthScale | Int32 | Échelle de la largeur de l'image, en pourcentage. |
| heightScale | Int32 | Échelle de la hauteur de l'image, en pourcentage. |

### Valeur de retour

Renvoie un objet Picture.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts; // Added this using directive
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class ShapeCollectionMethodAddPictureInChartWithInt32Int32StreamInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 15, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);
            chart.NSeries.CategoryData = "B1:B3";

            // Créer un flux mémoire avec les données d'image
            byte[] imageData = File.ReadAllBytes("example.jpg");
            MemoryStream stream = new MemoryStream(imageData);

            try
            {
                // Appeler AddPictureInChart avec les paramètres (Int32, Int32, Stream, Int32, Int32)
                Picture picture = chart.Shapes.AddPictureInChart(100, 100, stream, 50, 50);
                
                Console.WriteLine("Picture added to chart successfully. Original dimensions: " + 
                    $"{picture.OriginalWidth}x{picture.OriginalHeight}");
                
                // Enregistrez le classeur
                workbook.Save("AddPictureInChartDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddPictureInChart method: {ex.Message}");
            }
            finally
            {
                stream.Dispose();
            }
        }
    }
}
```

### Voir aussi

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


