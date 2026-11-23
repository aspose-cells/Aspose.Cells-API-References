---
title: "Enum ColorDepth"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Rendering.ColorDepth enum. Énumère le type de profondeur de bits pour l'image tiff"
type: docs
url: /fr/net/aspose.cells.rendering/colordepth/
---
## ColorDepth enumeration

Énumère le type de profondeur de bits pour l'image tiff.

```csharp
public enum ColorDepth
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Default | `0` | Valeur par défaut, valeur non définie. |
| Format1bpp | `1` | 1 bit par pixel |
| Format4bpp | `4` | 4 bits par pixel |
| Format8bpp | `8` | 8 bits par pixel |
| Format24bpp | `24` | 24 bits par pixel |
| Format32bpp | `32` | 32 bits par pixel |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Drawing;
    using System;

    public class RenderingClassColorDepthDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("TIFF Color Depth Demonstration");
            worksheet.Cells["B2"].PutValue(12345);
            
            // Configurer les options d'image TIFF
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Tiff;
            options.TiffColorDepth = ColorDepth.Format8bpp;

            // Rendre la feuille de calcul en TIFF avec la profondeur de couleur spécifiée
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "output_8bpp.tiff");

            // Démontrer une autre variante de profondeur de couleur
            options.TiffColorDepth = ColorDepth.Format24bpp;
            renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "output_24bpp.tiff");

            Console.WriteLine("TIFF files created with different color depths.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


