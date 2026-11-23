---
title: "PictureBulletValue.ImageData"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PictureBulletValue. Obtient et définit les données d'image du puce"
type: docs
url: /fr/net/aspose.cells.drawing.texts/picturebulletvalue/imagedata/
---
## PictureBulletValue.ImageData property

Obtient et définit les données d'image de la puce.

```csharp
public byte[] ImageData { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;
    using System.IO;

    public class PictureBulletValuePropertyImageDataDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Créez une instance de PictureBulletValue
                PictureBulletValue bulletValue = new PictureBulletValue();
                
                // Démontrez la définition et la récupération d'ImageData
                byte[] sampleImageData = new byte[] { 0x01, 0x02, 0x03 }; // Sample data
                bulletValue.ImageData = sampleImageData;
                
                // Affichez la valeur de la propriété ImageData
                Console.WriteLine("ImageData length: " + (bulletValue.ImageData?.Length ?? 0) + " bytes");
                
                // Affichez la propriété Type (lecture seule)
                Console.WriteLine("Bullet Type: " + bulletValue.Type);
                
                // Enregistrez le classeur
                workbook.Save("PictureBulletValueImageDataDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [PictureBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


