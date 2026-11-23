---
title: "SheetRender.GetPageSizeInch"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SheetRender. Obtenez la taille de page en pouces de l'image de sortie"
type: docs
url: /fr/net/aspose.cells.rendering/sheetrender/getpagesizeinch/
---
## SheetRender.GetPageSizeInch method

Obtenir la taille de page en pouces de l’image de sortie.

```csharp
public float[] GetPageSizeInch(int pageIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | L'index de la page est basé sur zéro. |

### Valeur de retour

Taille de l'image, [0] pour la largeur et [1] pour la hauteur

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SheetRenderMethodGetPageSizeInchWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.PageSetup.PrintArea = "A1:D10";
            worksheet.PageSetup.LeftMargin = 0;
            worksheet.PageSetup.RightMargin = 0;
            worksheet.PageSetup.TopMargin = 0;
            worksheet.PageSetup.BottomMargin = 0;

            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                OnePagePerSheet = true,
                ImageType = ImageType.Png
            };

            SheetRender sheetRender = new SheetRender(worksheet, options);
            float[] pageSize = sheetRender.GetPageSizeInch(0);
            
            Console.WriteLine($"Page Size (Inches): Width={pageSize[0]}, Height={pageSize[1]}");
        }
    }
}
```

### Voir aussi

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


