---
title: "ImageOrPrintOptions.OnlyArea"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ImageOrPrintOptions. Si cette propriété est vraie, une zone sera générée et aucune mise à l'échelle ne sera appliquée"
type: docs
url: /fr/net/aspose.cells.rendering/imageorprintoptions/onlyarea/
---
## ImageOrPrintOptions.OnlyArea property

Si cette propriété est vraie, une zone sera exportée et aucune échelle ne sera appliquée.

```csharp
public bool OnlyArea { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyOnlyAreaDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple aux cellules
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Définir les options d'image avec la propriété OnlyArea
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.OnlyArea = true; // Only render the used area

            // Rendre la feuille de calcul en image
            SheetRender sr = new SheetRender(worksheet, options);
            using (MemoryStream ms = new MemoryStream())
            {
                sr.ToImage(0, ms);
                Console.WriteLine("Worksheet rendered to image with OnlyArea=true");
            }
        }
    }
}
```

### Voir aussi

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


