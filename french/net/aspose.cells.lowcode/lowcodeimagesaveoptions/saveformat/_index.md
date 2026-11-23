---
title: "LowCodeImageSaveOptions.SaveFormat"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LowCodeImageSaveOptions. Obtient ou définit le format d'enregistrement"
type: docs
url: /fr/net/aspose.cells.lowcode/lowcodeimagesaveoptions/saveformat/
---
## LowCodeImageSaveOptions.SaveFormat property

Obtient ou définit le format d’enregistrement.

```csharp
public override SaveFormat SaveFormat { get; set; }
```

### Remarques

Si [`ImageOptions`](../imageoptions/) a été spécifié, la définition de cette propriété modifiera également la valeur [`ImageType`](../../../aspose.cells.rendering/imageorprintoptions/imagetype/) de celle-ci.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeImageSaveOptionsPropertySaveFormatDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells LowCode Image SaveFormat Demo");

            // Initialisez LowCodeImageSaveOptions avec les valeurs par défaut
            LowCodeImageSaveOptions options = new LowCodeImageSaveOptions();
            
            // Affichez le SaveFormat initial (par défaut est Png)
            Console.WriteLine("Initial SaveFormat: " + options.SaveFormat);

            // Configurez la sortie JPEG
            options.SaveFormat = SaveFormat.Jpg;
            options.ImageOptions = new ImageOrPrintOptions
            {
                Quality = 85,
                OnePagePerSheet = true,
                ImageType = ImageType.Jpeg
            };
            SaveWorksheetAsImage(worksheet, options, "output_initial.jpg");

            // Changez au format PNG et enregistrez à nouveau
            options.SaveFormat = SaveFormat.Png;
            options.ImageOptions.ImageType = ImageType.Png;
            Console.WriteLine("\nModified SaveFormat: " + options.SaveFormat);
            SaveWorksheetAsImage(worksheet, options, "output_modified.png");
        }

        private static void SaveWorksheetAsImage(Worksheet worksheet, LowCodeImageSaveOptions options, string fileName)
        {
            // Rendez la feuille de calcul en utilisant les options configurées
            SheetRender renderer = new SheetRender(worksheet, options.ImageOptions);
            renderer.ToImage(0, fileName);
            Console.WriteLine($"Saved: {fileName}");
        }
    }
}
```

### Voir aussi

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [LowCodeImageSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


