---
title: "PicFormatOption.Bottom"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PicFormatOption. Obtient ou définit le décalage inférieur pour l’étirement de l’image"
type: docs
url: /fr/net/aspose.cells.drawing/picformatoption/bottom/
---
## PicFormatOption.Bottom property

Obtient ou définit le décalage inférieur pour l'étirement de l'image.

```csharp
public double Bottom { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PicFormatOptionPropertyBottomDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Utilisez un fichier image existant (remplacez par le chemin réel de l’image)
            string imagePath = "sample.jpg";

            // Ajouter une forme rectangle à la feuille de calcul
            Shape shape = worksheet.Shapes.AddRectangle(5, 5, 0, 0, 200, 200);

            // Configurer le remplissage de la forme pour utiliser l’image d’exemple
            // FillType est déduit en définissant ImageData, ce qui définit le type sur Texture
            shape.FillFormat.ImageData = File.ReadAllBytes(imagePath);
            
            // Créer et configurer les options de format d’image
            PicFormatOption picFormat = new PicFormatOption();
            picFormat.Type = FillPictureType.Stretch;

            // Afficher la valeur initiale Bottom
            Console.WriteLine("Initial Bottom value: " + picFormat.Bottom);

            // Modifier le décalage Bottom et afficher la nouvelle valeur
            picFormat.Bottom = 0.3;
            Console.WriteLine("Modified Bottom value: " + picFormat.Bottom);

            // Associer le PicFormatOption au remplissage de la forme (en supposant applicable)
            // Remarque : cette étape peut nécessiter des méthodes spécifiques à l’API non montrées dans le contexte fourni
            // À titre de démonstration, le PicFormatOption est créé et configuré

            // Enregistrez le classeur avec les modifications appliquées
            workbook.Save("PicFormatOptionBottomDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


