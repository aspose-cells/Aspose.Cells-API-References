---
title: "PageSetup.SetHeaderPicture"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PageSetup. Définit une image dans l'en-tête d'une feuille de calcul"
type: docs
url: /fr/net/aspose.cells/pagesetup/setheaderpicture/
---
## PageSetup.SetHeaderPicture method

Définit une image dans l'en-tête d'une feuille de calcul.

```csharp
public Picture SetHeaderPicture(int section, byte[] headerPicture)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| section | Int32 | 0 : Section gauche, 1 : Section centrale, 2 : Section droite. |
| headerPicture | Byte[] | Données d'image. |

### Valeur de retour

Renvoie [`Picture`](../../../aspose.cells.drawing/picture/) objet.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PageSetupMethodSetHeaderPictureWithInt32ByteArrayDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Chargez un fichier image dans un tableau d'octets
            byte[] headerImageBytes = File.ReadAllBytes("header_logo.png");
            
            try
            {
                // Appelez SetHeaderPicture avec l'index de section (0 pour l'en-tête central) et les octets d'image
                Picture picture = worksheet.PageSetup.SetHeaderPicture(0, headerImageBytes);
                
                // Définir le script d'en-tête pour afficher l'image
                worksheet.PageSetup.SetHeader(0, "&G");
                
                Console.WriteLine("SetHeaderPicture method executed successfully with parameters (Int32, Byte[])");
                Console.WriteLine($"Picture dimensions: {picture.OriginalWidth}x{picture.OriginalHeight} pixels");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetHeaderPicture method: {ex.Message}");
            }
            
            // Enregistrez le classeur
            workbook.Save("SetHeaderPictureDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Picture](../../../aspose.cells.drawing/picture/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


