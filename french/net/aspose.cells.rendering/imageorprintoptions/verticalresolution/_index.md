---
title: "ImageOrPrintOptions.VerticalResolution"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ImageOrPrintOptions. Obtient ou définit la résolution verticale des images générées en points par pouce"
type: docs
url: /fr/net/aspose.cells.rendering/imageorprintoptions/verticalresolution/
---
## ImageOrPrintOptions.VerticalResolution property

Obtient ou définit la résolution verticale des images générées, en points par pouce.

```csharp
public int VerticalResolution { get; set; }
```

### Remarques

La valeur par défaut est 96.

Le réglage de [`HorizontalResolution`](../horizontalresolution/) et de `VerticalResolution` affecte la largeur et la hauteur de l'image de sortie en pixels.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyVerticalResolutionDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple et créer un graphique
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B3"].PutValue(200);
            
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Créer des options d'image avec une résolution verticale spécifique
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Png;
            options.VerticalResolution = 300; // Setting vertical resolution to 300 DPI
            options.HorizontalResolution = 300; // For consistency, setting horizontal resolution too

            // Enregistrer le graphique en tant qu'image avec la résolution spécifiée
            chart.ToImage("output_chart.png", options);
            
            Console.WriteLine("Chart saved as image with vertical resolution of 300 DPI.");
        }
    }
}
```

### Voir aussi

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


