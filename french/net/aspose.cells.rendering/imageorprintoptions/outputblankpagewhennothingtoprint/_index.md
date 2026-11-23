---
title: "ImageOrPrintOptions.OutputBlankPageWhenNothingToPrint"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ImageOrPrintOptions. Indique s’il faut générer une page blanche lorsqu’il n’y a rien à imprimer"
type: docs
url: /fr/net/aspose.cells.rendering/imageorprintoptions/outputblankpagewhennothingtoprint/
---
## ImageOrPrintOptions.OutputBlankPageWhenNothingToPrint property

Indique s'il faut générer une page blanche lorsqu'il n'y a rien à imprimer.

```csharp
public bool OutputBlankPageWhenNothingToPrint { get; set; }
```

### Remarques

La valeur par défaut est false.

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyOutputBlankPageWhenNothingToPrintDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur vide
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul qui est vide
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir les options d’image ou d’impression
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.OnePagePerSheet = true;
            
            // Démontrer la propriété OutputBlankPageWhenNothingToPrint
            options.OutputBlankPageWhenNothingToPrint = true;
            
            // Rendre la feuille
            SheetRender renderer = new SheetRender(worksheet, options);
            
            // La sortie produira toujours une page blanche en raison du paramètre de la propriété
            Console.WriteLine("Page count with OutputBlankPageWhenNothingToPrint=true: " + renderer.PageCount);
            
            // Enregistrer la première page dans le flux mémoire
            MemoryStream stream = new MemoryStream();
            renderer.ToImage(0, stream);
            Console.WriteLine("Image data length: " + stream.ToArray().Length);
            
            // Définir maintenant la propriété sur false
            options.OutputBlankPageWhenNothingToPrint = false;
            SheetRender renderer2 = new SheetRender(worksheet, options);
            
            // La sortie aura maintenant zéro page
            Console.WriteLine("Page count with OutputBlankPageWhenNothingToPrint=false: " + renderer2.PageCount);
        }
    }
}
```

### Voir aussi

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


