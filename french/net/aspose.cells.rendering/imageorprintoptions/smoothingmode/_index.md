---
title: "ImageOrPrintOptions.SmoothingMode"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ImageOrPrintOptions. Spécifie si l'anticrénelage de lissage est appliqué aux lignes et courbes ainsi qu'aux bords des zones remplies. La valeur par défaut est SmoothingMode.None"
type: docs
url: /fr/net/aspose.cells.rendering/imageorprintoptions/smoothingmode/
---
## ImageOrPrintOptions.SmoothingMode property

Spécifie si le lissage (antialiasing) est appliqué aux lignes et courbes ainsi qu'aux bords des zones remplies. La valeur par défaut est SmoothingMode.None

```csharp
public SmoothingMode SmoothingMode { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class ImageOrPrintOptionsPropertySmoothingModeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].Value = "ImageOrPrintOptions Demo";
            worksheet.Cells["A2"].Value = "Sample Data";

            try
            {
                // Créer une instance de ImageOrPrintOptions
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Afficher certaines des propriétés disponibles
                Console.WriteLine("HorizontalResolution: " + options.HorizontalResolution);
                Console.WriteLine("VerticalResolution: " + options.VerticalResolution);
                Console.WriteLine("ImageType: " + options.ImageType);

                // Créer un SheetRender pour démontrer la propriété
                SheetRender renderer = new SheetRender(worksheet, options);

                // Rendre vers un flux mémoire pour démontrer la fonctionnalité
                MemoryStream stream = new MemoryStream();
                renderer.ToImage(0, stream);

                Console.WriteLine("Sheet rendered successfully");
                Console.WriteLine("Image size: " + stream.Length + " bytes");

                // Enregistrez le classeur
                workbook.Save("ImageOrPrintOptionsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


