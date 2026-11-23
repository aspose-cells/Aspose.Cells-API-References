---
title: "PageSetup.SetPicture"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PageSetup. Définit une image dans l'en-tête/pied de page d'une feuille de calcul"
type: docs
url: /fr/net/aspose.cells/pagesetup/setpicture/
---
## PageSetup.SetPicture method

Définit une image dans l'en-tête/pied de page d'une feuille de calcul.

```csharp
public Picture SetPicture(bool isFirst, bool isEven, bool isHeader, int section, byte[] imageData)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| isFirst | Boolean | Indique si l'image de l'en-tête/pied de page de la première page est définie. |
| isEven | Boolean | Indique si l'image de l'en-tête/pied de page des pages paires est définie. |
| isHeader | Boolean | Indique si l'image de l'en-tête/pied de page est définie. |
| section | Int32 | 0 : Section gauche, 1 : Section centrale, 2 : Section droite. |
| imageData | Byte[] | Données d'image. |

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

    public class PageSetupMethodSetPictureWithBooleanBooleanBooleanInt32ByteDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Chargez un fichier image dans un tableau d'octets
            byte[] imageData = File.ReadAllBytes("example.jpg");

            try
            {
                // Appelez la méthode SetPicture pour définir l'image d'en-tête
                // Paramètres : isFirstPage, isEvenPage, isHeader, section, imageData
                Picture picture = pageSetup.SetPicture(false, false, true, 1, imageData);

                // Définir le texte d'en-tête
                pageSetup.SetHeader(1, "&G");
                
                Console.WriteLine("SetPicture method executed successfully. Header image set.");

                // Enregistrez le classeur
                workbook.Save("PageSetupSetPictureDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetPicture method: {ex.Message}");
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


