---
title: "ConditionalFormattingIcon.GetIconImageData"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ConditionalFormattingIcon. Obtenir les données du jeu d'icônes"
type: docs
url: /fr/net/aspose.cells/conditionalformattingicon/geticonimagedata/
---
## ConditionalFormattingIcon.GetIconImageData method

Obtenir les données du jeu d'icônes

```csharp
public static byte[] GetIconImageData(IconSetType type, int index)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | IconSetType | type de l'icône |
| indice | Int32 | index de l'icône |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class ConditionalFormattingIconMethodGetIconImageDataWithIconSetTypeInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Pas besoin de créer une instance puisque GetIconImageData est statique
            
            try
            {
                // Appeler GetIconImageData avec IconSetType.Arrows3 et l'index 0
                byte[] imageData = ConditionalFormattingIcon.GetIconImageData(IconSetType.Arrows3, 0);
                
                Console.WriteLine("Method executed successfully. Image data length: " + imageData.Length);
                
                // Enregistrer les données d'image dans un fichier à des fins de démonstration
                File.WriteAllBytes("icon_image.png", imageData);
                Console.WriteLine("Icon image saved to icon_image.png");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetIconImageData method: {ex.Message}");
            }
            
            // Enregistrez le classeur
            workbook.Save("ConditionalFormattingIconGetIconImageDataDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [IconSetType](../../iconsettype/)
* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


