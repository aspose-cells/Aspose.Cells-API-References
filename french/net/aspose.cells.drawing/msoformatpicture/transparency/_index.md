---
title: "MsoFormatPicture.Transparency"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MsoFormatPicture. Retourne ou définit le degré de transparence de la zone comme une valeur de 0,0 opaque à 1,0 claire"
type: docs
url: /fr/net/aspose.cells.drawing/msoformatpicture/transparency/
---
## MsoFormatPicture.Transparency property

Renvoie ou définit le degré de transparence de la zone comme une valeur de 0,0 (opaque) à 1,0 (transparent).

```csharp
public double Transparency { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyTransparencyDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter deux images à la feuille de calcul
            int index1 = worksheet.Pictures.Add(0, 0, "image1.png");
            int index2 = worksheet.Pictures.Add(2, 0, "image2.png");

            // Définir la transparence pour les images
            worksheet.Pictures[index1].FormatPicture.Transparency = 0.5;
            worksheet.Pictures[index2].FormatPicture.Transparency = 0.69;

            // Enregistrer et recharger le classeur pour vérifier les paramètres de transparence
            string outputPath = "output.xlsx";
            workbook.Save(outputPath);
            
            Workbook loadedWorkbook = new Workbook(outputPath);
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];

            // Afficher les valeurs de transparence dans la console
            Console.WriteLine("Picture 1 Transparency: " + loadedWorksheet.Pictures[0].FormatPicture.Transparency);
            Console.WriteLine("Picture 2 Transparency: " + loadedWorksheet.Pictures[1].FormatPicture.Transparency);
        }
    }
}
```

### Voir aussi

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


