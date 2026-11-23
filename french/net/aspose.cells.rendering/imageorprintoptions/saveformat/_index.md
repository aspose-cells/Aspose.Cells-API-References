---
title: "ImageOrPrintOptions.SaveFormat"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ImageOrPrintOptions. Obtient ou définit le type de format de fichier de sortie. Prise en charge Tiff/XPS"
type: docs
url: /fr/net/aspose.cells.rendering/imageorprintoptions/saveformat/
---
## ImageOrPrintOptions.SaveFormat property

Obtient ou définit le type de format de fichier de sortie. Prise en charge Tiff/XPS

```csharp
[Obsolete("For Tiff/Svg, use ImageType; For Xps, use Workbook.Save(string, SaveOptions) with XpsSaveOptions")]
[EditorBrowsable(EditorBrowsableState.Never)]
public SaveFormat SaveFormat { get; set; }
```

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, pour Tiff/Svg, utilisez [`ImageType`](../imagetype/) ; pour Xps, utilisez [`Save`](../../../aspose.cells/workbook/save/) avec [`XpsSaveOptions`](../../../aspose.cells/xpssaveoptions/). Cette propriété sera supprimée 12 mois plus tard, depuis août 2022. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class ImageOrPrintOptionsPropertySaveFormatDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur et remplir avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells SaveFormat Demonstration");
            
            // Créer une instance de ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            // Afficher la valeur initiale de SaveFormat
            Console.WriteLine("Initial SaveFormat: " + options.SaveFormat);

            // Définir SaveFormat sur TIFF et rendre la feuille de calcul
            options.SaveFormat = SaveFormat.Tiff;
            SheetRender tiffRenderer = new SheetRender(worksheet, options);
            using (FileStream tiffStream = new FileStream("output.tiff", FileMode.Create))
            {
                tiffRenderer.ToTiff(tiffStream);
            }
            Console.WriteLine("Rendered worksheet to TIFF format");

            // Modifier SaveFormat en XPS et rendre à nouveau
            options.SaveFormat = SaveFormat.Xps;
            SheetRender xpsRenderer = new SheetRender(worksheet, options);
            using (FileStream xpsStream = new FileStream("output.xps", FileMode.Create))
            {
                // Note : SheetRender ne prend pas en charge le format XPS. Cela sera enregistré au format image à la place.
                xpsRenderer.ToImage(0, xpsStream);
            }
            Console.WriteLine("Rendered worksheet to XPS format");
        }
    }
}
```

### Voir aussi

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


