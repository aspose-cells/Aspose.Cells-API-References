---
title: "PicFormatOption.Top"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PicFormatOption. Obtient ou définit le décalage supérieur pour l’étirement de l’image"
type: docs
url: /fr/net/aspose.cells.drawing/picformatoption/top/
---
## PicFormatOption.Top property

Obtient ou définit le décalage supérieur pour l'étirement de l'image.

```csharp
public double Top { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PicFormatOptionPropertyTopDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Utilisez une image existante ou fournissez le chemin d’image correct
            string imagePath = "existingImage.png";

            // Ajouter une forme avec les paramètres corrects
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 200, 200);
            
            // Appliquer un remplissage d’image en utilisant ImageData
            shape.FillFormat.ImageData = File.ReadAllBytes(imagePath);

            // Créer et configurer PicFormatOption directement
            PicFormatOption picFormat = new PicFormatOption();

            Console.WriteLine("Initial Top value: " + picFormat.Top);
            picFormat.Top = 0.3;

            // En supposant que PicFormatOption doit être associé au format de remplissage
            // Cette partie peut nécessiter une implémentation spécifique à l’API non montrée dans les définitions de type
            // shape.FillFormat.SetPicFormatOption(picFormat);

            Console.WriteLine("Modified Top value: " + picFormat.Top);
            workbook.Save("TopPropertyDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


