---
title: "SheetRender.ToTiff"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SheetRender. Rendre toute la worksheet en image Tiff vers le flux"
type: docs
url: /fr/net/aspose.cells.rendering/sheetrender/totiff/
---
## ToTiff(Stream) {#totiff}

Rendre toute la feuille de calcul en image Tiff vers le flux.

```csharp
public void ToTiff(Stream stream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| stream | Stream | le flux de l'image de sortie |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SheetRenderMethodToTiffWithStreamDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur et accéder à la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez du contenu d'exemple pour démontrer le rendu
            worksheet.Cells["A1"].PutValue("Aspose.Cells TIFF Rendering Demo");
            
            // Configurez les options d'image pour le rendu
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;

            // Créez le rendu de feuille avec les options configurées
            SheetRender renderer = new SheetRender(worksheet, options);
            try
            {
                // Créez un flux de sortie pour l'image TIFF
                using (FileStream tiffStream = new FileStream("output.tiff", FileMode.Create))
                {
                    // Rendez la worksheet en TIFF en utilisant le flux
                    renderer.ToTiff(tiffStream);
                    Console.WriteLine("Worksheet successfully rendered to TIFF stream.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during TIFF rendering: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToTiff(string) {#totiff_1}

Rendre toute la feuille de calcul en image Tiff vers un fichier.

```csharp
public void ToTiff(string filename)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| nom de fichier | String | le nom de fichier de l'image de sortie |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderMethodToTiffWithStringDemo
    {
        public static void Run()
        {
            // Charger le fichier Excel source
            Workbook workbook = new Workbook("Book1.xlsx");

            // Créer des options d'image ou d'impression
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.SaveFormat = SaveFormat.Tiff;

            // Créer un rendu de feuille pour la première feuille de calcul
            SheetRender sheetRender = new SheetRender(workbook.Worksheets[0], options);

            // Enregistrez toutes les pages de la feuille en tant que fichier TIFF multi-pages
            sheetRender.ToTiff("output.tiff");
        }
    }
}
```

### Voir aussi

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


