---
title: "Enum ImageType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.ImageType enum. Spécifie le format de type d’une image"
type: docs
url: /fr/net/aspose.cells.drawing/imagetype/
---
## ImageType enumeration

Spécifie le type (format) d'une image.

```csharp
public enum ImageType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Unknown | `0` | Un type d'image inconnu. |
| Emf | `2` | Metafile Windows amélioré. |
| Wmf | `3` | Metafile Windows. |
| Pict | `4` | Macintosh PICT. |
| Jpeg | `5` | JPEG JFIF. |
| Png | `6` | Portable Network Graphics. |
| Bmp | `7` | Bitmap Windows |
| Gif | `66` | Gif |
| Tiff | `67` | Tiff |
| Svg | `68` | Svg |
| Svm | `69` | Svm |
| Gltf | `70` | glTF |
| OfficeCompatibleEmf | `71` | Windows Enhanced Metafile qui est plus compatible avec Office. |
| WebP | `72` | Format d’image Weppy |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class ImageTypeDemo
    {
        public static void ImageTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données du graphique
            chart.SetChartDataRange("A1:B4", true);

            // Enregistrer le graphique en tant qu’image dans différents formats
            chart.ToImage("ChartImageEmf.emf", ImageType.Emf);
            chart.ToImage("ChartImageWmf.wmf", ImageType.Wmf);
            chart.ToImage("ChartImagePng.png", ImageType.Png);
            chart.ToImage("ChartImageJpeg.jpeg", ImageType.Jpeg);
            chart.ToImage("ChartImageBmp.bmp", ImageType.Bmp);
            chart.ToImage("ChartImageGif.gif", ImageType.Gif);
            chart.ToImage("ChartImageTiff.tiff", ImageType.Tiff);
            chart.ToImage("ChartImageSvg.svg", ImageType.Svg);

            // Afficher les résultats
            Console.WriteLine("Chart images saved in various formats.");

            // Enregistrez le classeur
            workbook.Save("ImageTypeExample.xlsx");
            workbook.Save("ImageTypeExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


