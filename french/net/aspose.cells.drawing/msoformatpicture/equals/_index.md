---
title: "MsoFormatPicture.Equals"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode MsoFormatPicture."
type: docs
url: /fr/net/aspose.cells.drawing/msoformatpicture/equals/
---
## MsoFormatPicture.Equals method

```csharp
public override bool Equals(object obj)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| obj | Object |  |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoFormatPictureMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter deux images à la feuille de calcul
            int pictureIndex1 = worksheet.Pictures.Add(0, 0, "example.jpg");
            int pictureIndex2 = worksheet.Pictures.Add(5, 0, "example.jpg");
            
            Picture picture1 = worksheet.Pictures[pictureIndex1];
            Picture picture2 = worksheet.Pictures[pictureIndex2];

            // Obtenir les objets MsoFormatPicture
            MsoFormatPicture format1 = picture1.FormatPicture;
            MsoFormatPicture format2 = picture2.FormatPicture;

            // Définissez différentes propriétés pour démontrer la comparaison d'égalité
            format1.Brightness = 0.5;
            format1.Contrast = 0.3;
            format2.Brightness = 0.5;
            format2.Contrast = 0.3;

            try
            {
                // Comparer les deux objets MsoFormatPicture
                bool areEqual = format1.Equals((object)format2);
                Console.WriteLine($"Format objects are equal: {areEqual}");

                // Modifier un format et comparer à nouveau
                format2.Brightness = 0.7;
                areEqual = format1.Equals((object)format2);
                Console.WriteLine($"After modification, format objects are equal: {areEqual}");

                // Comparer avec null
                bool isNullEqual = format1.Equals((object)null);
                Console.WriteLine($"Comparison with null: {isNullEqual}");

                // Comparer avec un type différent
                bool isDifferentTypeEqual = format1.Equals((object)"string");
                Console.WriteLine($"Comparison with different type: {isDifferentTypeEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Enregistrez le classeur
            workbook.Save("MsoFormatPictureMethodEqualsWithObjectDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


