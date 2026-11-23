---
title: "PageSetup.SetFooterPicture"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PageSetup. Définit une image dans le pied de page d'une feuille de calcul"
type: docs
url: /fr/net/aspose.cells/pagesetup/setfooterpicture/
---
## PageSetup.SetFooterPicture method

Définit une image dans le pied de page d'une feuille de calcul.

```csharp
public Picture SetFooterPicture(int section, byte[] footerPicture)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| section | Int32 | 0 : Section gauche, 1 : Section centrale, 2 : Section droite. |
| footerPicture | Byte[] | Données d'image. |

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

    public class PageSetupMethodSetFooterPictureWithInt32ByteArrayDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Chargez un fichier image dans un tableau d'octets
            byte[] footerImageData = File.ReadAllBytes("footer_logo.png");
            
            try
            {
                // Appelez la méthode SetFooterPicture avec l'index de section (0 pour le centre, 1 pour la gauche, 2 pour la droite) et les données d'image
                Picture footerPicture = worksheet.PageSetup.SetFooterPicture(0, footerImageData);
                
                // Définissez le texte du pied de page à afficher avec l'image
                worksheet.PageSetup.SetFooter(0, "&G");
                
                Console.WriteLine("SetFooterPicture method executed successfully with parameters (Int32, Byte[])");
                
                // Enregistrez le classeur pour voir l'image du pied de page
                workbook.Save("PageSetupMethodSetFooterPictureWithInt32ByteArrayDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFooterPicture method: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [Picture](../../../aspose.cells.drawing/picture/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


