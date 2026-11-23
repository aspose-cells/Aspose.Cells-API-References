---
title: "ImageOrPrintOptions.EmfType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ImageOrPrintOptions. Obtient ou définit un EmfType qui spécifie le format du Metafile. La valeur par défaut est EmfPlusDual"
type: docs
url: /fr/net/aspose.cells.rendering/imageorprintoptions/emftype/
---
## ImageOrPrintOptions.EmfType property

Obtient ou définit un EmfType qui spécifie le format du Metafile. La valeur par défaut est EmfPlusDual.

```csharp
public EmfType EmfType { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class ImageOrPrintOptionsPropertyEmfTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["A2"].Value = "EMF Type Demo";

            try
            {
                // Créer une instance de ImageOrPrintOptions
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Définir le type d’image sur EMF
                options.ImageType = Aspose.Cells.Drawing.ImageType.Emf;

                // Créer SheetRender avec les options
                SheetRender renderer = new SheetRender(worksheet, options);

                // Enregistrer au format EMF
                using (MemoryStream stream = new MemoryStream())
                {
                    renderer.ToImage(0, stream);

                    // Afficher la valeur de la propriété EmfType
                    Console.WriteLine("EmfType value: " + options.EmfRenderSetting);

                    // Enregistrer le fichier EMF
                    File.WriteAllBytes("output.emf", stream.ToArray());
                    Console.WriteLine("EMF file created successfully.");
                }
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


