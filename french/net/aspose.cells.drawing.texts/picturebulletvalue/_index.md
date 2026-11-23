---
title: "Classe PictureBulletValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.Texts.PictureBulletValue classe. Représente la valeur de la puce d'image"
type: docs
url: /fr/net/aspose.cells.drawing.texts/picturebulletvalue/
---
## PictureBulletValue class

Représente la valeur de la puce image.

```csharp
public class PictureBulletValue : BulletValue
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [PictureBulletValue](picturebulletvalue/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [ImageData](../../aspose.cells.drawing.texts/picturebulletvalue/imagedata/) { get; set; } | Obtient et définit les données d'image de la puce. |
| override [Type](../../aspose.cells.drawing.texts/picturebulletvalue/type/) { get; } | Obtient le type de la valeur de la puce. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;
    using System.IO;

    public class TextsClassPictureBulletValueDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Crée une instance de la classe PictureBulletValue
                PictureBulletValue bulletValue = new PictureBulletValue();
                
                // Charge des données d'image d'exemple (remplacez par le chemin réel de l'image)
                string imagePath = "sample.png";
                if (File.Exists(imagePath))
                {
                    bulletValue.ImageData = File.ReadAllBytes(imagePath);
                    
                    // Afficher les informations de base
                    Console.WriteLine($"PictureBulletValue created with Type: {bulletValue.Type}");
                    Console.WriteLine($"Image data length: {bulletValue.ImageData?.Length ?? 0} bytes");
                }
                else
                {
                    Console.WriteLine("Sample image not found, using empty bullet value");
                }
                
                // Enregistrez le classeur
                workbook.Save("PictureBulletValueDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with PictureBulletValue: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [BulletValue](../bulletvalue/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


