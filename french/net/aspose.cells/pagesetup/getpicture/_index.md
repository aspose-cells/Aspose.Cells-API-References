---
title: "PageSetup.GetPicture"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PageSetup. Obtient l'objet Picture de l'en-tête / pied de page"
type: docs
url: /fr/net/aspose.cells/pagesetup/getpicture/
---
## GetPicture(bool, int) {#getpicture_1}

Obtient l'objet [`Picture`](../../../aspose.cells.drawing/picture/) de l'en-tête / pied de page.

```csharp
public Picture GetPicture(bool isHeader, int section)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| isHeader | Boolean | Indique s'il se trouve dans l'en-tête ou le pied de page. |
| section | Int32 | 0 : Section gauche, 1 : Section centrale, 2 : Section droite. |

### Valeur de retour

Renvoie l'objet [`Picture`](../../../aspose.cells.drawing/picture/). Renvoie null s'il n'y a pas d'image.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PageSetupMethodGetPictureWithBooleanInt32Demo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez une image à l'en-tête de la feuille de calcul
            byte[] imageData = System.IO.File.ReadAllBytes("header.png");
            worksheet.PageSetup.SetHeaderPicture(0, imageData);
            
            // Obtenez l'image de l'en-tête et modifiez sa luminosité
            Picture headerPicture = worksheet.PageSetup.GetPicture(true, 0);
            headerPicture.FormatPicture.Brightness = 50;
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Picture](../../../aspose.cells.drawing/picture/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetPicture(bool, bool, bool, int) {#getpicture}

Obtient l'objet [`Picture`](../../../aspose.cells.drawing/picture/) de l'en-tête / pied de page.

```csharp
public Picture GetPicture(bool isFirst, bool isEven, bool isHeader, int section)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| isFirst | Boolean | Indique si l'on récupère l'image de l'en-tête/pied de page de la première page. |
| isEven | Boolean | Indique si l'on récupère l'image de l'en-tête/pied de page des pages paires. |
| isHeader | Boolean | Indique si l'on récupère l'image de l'en-tête/pied de page. |
| section | Int32 | 0 : Section gauche, 1 : Section centrale, 2 : Section droite. |

### Valeur de retour

Renvoie [`Picture`](../../../aspose.cells.drawing/picture/) objet.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class PageSetupMethodGetPictureWithBooleanBooleanBooleanInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtenir l'objet PageSetup
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Définissez certaines propriétés d'en-tête/pied de page pour garantir que nous disposons d'images à récupérer
            pageSetup.IsHFDiffFirst = true;
            pageSetup.IsHFDiffOddEven = true;
            
            try
            {
                // Appelez la méthode GetPicture avec les paramètres : isFirst, isEven, isHeader, section
                // Vérification de l'en-tête de la première page (section 0 - en-tête central)
                Picture picture = pageSetup.GetPicture(true, false, true, 0);
                
                if (picture != null)
                {
                    Console.WriteLine("Retrieved picture from first page header:");
                    Console.WriteLine($"Original dimensions: {picture.OriginalWidth}x{picture.OriginalHeight}");
                }
                else
                {
                    Console.WriteLine("No picture found in first page header");
                }
                
                // Enregistrez le classeur
                workbook.Save("PageSetupGetPictureDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetPicture method: {ex.Message}");
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


