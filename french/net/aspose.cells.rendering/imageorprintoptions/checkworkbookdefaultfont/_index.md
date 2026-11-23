---
title: "ImageOrPrintOptions.CheckWorkbookDefaultFont"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ImageOrPrintOptions. Lorsque les caractères dans Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, ils peuvent apparaître sous forme de blocs dans le pdfimage. Réglez cette propriété sur true pour essayer d'utiliser la police par défaut du classeur afin d'afficher ces caractères en premier."
type: docs
url: /fr/net/aspose.cells.rendering/imageorprintoptions/checkworkbookdefaultfont/
---
## ImageOrPrintOptions.CheckWorkbookDefaultFont property

Lorsque les caractères dans le fichier Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, ils peuvent apparaître sous forme de blocs dans le PDF, l'image. Réglez ceci sur true pour essayer d'utiliser la police par défaut du classeur afin d'afficher ces caractères en premier.

```csharp
public bool CheckWorkbookDefaultFont { get; set; }
```

### Remarques

La valeur par défaut est vraie.

### Exemples

```csharp
using System;
using System.IO;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyCheckWorkbookDefaultFontDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue("Sample Text");
            
            // Définir la police par défaut pour le classeur
            workbook.DefaultStyle.Font.Name = "Arial";
            workbook.DefaultStyle.Font.Size = 12;

            // Créer des options d'image ou d'impression
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.OnePagePerSheet = true;
            
            // Activer la vérification de la police par défaut du classeur
            options.CheckWorkbookDefaultFont = true;

            // Rendre la feuille de calcul en image
            SheetRender renderer = new SheetRender(sheet, options);
            using (MemoryStream stream = new MemoryStream())
            {
                renderer.ToImage(0, stream);
                
                // Enregistrer l'image dans un fichier
                using (FileStream file = new FileStream("output.png", FileMode.Create))
                {
                    stream.WriteTo(file);
                }
            }
            
            Console.WriteLine("Image generated with workbook default font check.");
        }
    }
}
```

### Voir aussi

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


