---
title: "ImageOrPrintOptions.SetDesiredSize"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ImageOrPrintOptions. Définit la largeur et la hauteur souhaitées de l'image"
type: docs
url: /fr/net/aspose.cells.rendering/imageorprintoptions/setdesiredsize/
---
## SetDesiredSize(int, int) {#setdesiredsize}

Définit la largeur et la hauteur souhaitées de l'image.

```csharp
[Obsolete("Use SetDesiredSize(int, int, bool) by setting param keepAspectRatio to false instead.")]
public void SetDesiredSize(int desiredWidth, int desiredHeight)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| desiredWidth | Int32 | largeur souhaitée en pixels |
| desiredHeight | Int32 | hauteur souhaitée en pixels |

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser `SetDesiredSize` en définissant le paramètre keepAspectRatio sur false. Cette propriété sera supprimée 12 mois plus tard, depuis mai 2023. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsMethodSetDesiredSizeWithInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Sample Data");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue(i);
            }

            // Définir la zone d'impression
            worksheet.PageSetup.PrintArea = "A1:A11";

            // Créer des options d’image
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;
            options.SetDesiredSize(800, 600); // Using SetDesiredSize with Int32 parameters
            options.ImageType = Aspose.Cells.Drawing.ImageType.Jpeg;

            // Rendre la feuille de calcul en image
            SheetRender render = new SheetRender(worksheet, options);
            render.ToImage(0, "output.jpg");

            Console.WriteLine("Image generated with desired size 800x600");
        }
    }
}
```

### Voir aussi

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## SetDesiredSize(int, int, bool) {#setdesiredsize_1}

Définit la largeur et la hauteur souhaitées de l'image.

```csharp
public void SetDesiredSize(int desiredWidth, int desiredHeight, bool keepAspectRatio)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| desiredWidth | Int32 | largeur souhaitée en pixels |
| desiredHeight | Int32 | hauteur souhaitée en pixels |
| keepAspectRatio | Boolean | indique si le rapport d'aspect de l'image d'origine doit être conservé |

### Remarques

La largeur et la hauteur de l'image de sortie en pixels seront uniquement basées sur la largeur et la hauteur souhaitées définies.

Les [`HorizontalResolution`](../horizontalresolution/) et [`VerticalResolution`](../verticalresolution/) n'affecteront pas la largeur et la hauteur de l'image de sortie dans ce cas.

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsMethodSetDesiredSizeWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple et créer un graphique
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);
            chart.NSeries.CategoryData = "B1:B3";

            // Obtenir la forme du graphique
            Shape chartShape = worksheet.Shapes[0];

            // Définissez les options d’image
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Png;
            options.SetDesiredSize(800, 600, false); // Using SetDesiredSize with width, height, and keepAspectRatio

            // Enregistrer le graphique en tant qu'image
            MemoryStream stream = new MemoryStream();
            chartShape.ToImage(stream, options);

            // Enregistrer l'image dans un fichier
            File.WriteAllBytes("output_chart.png", stream.ToArray());
        }
    }
}
```

### Voir aussi

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


