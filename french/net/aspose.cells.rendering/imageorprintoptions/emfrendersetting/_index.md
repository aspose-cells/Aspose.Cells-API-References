---
title: "ImageOrPrintOptions.EmfRenderSetting"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ImageOrPrintOptions. Paramètre pour le rendu des métafichiers Emf dans le fichier source"
type: docs
url: /fr/net/aspose.cells.rendering/imageorprintoptions/emfrendersetting/
---
## ImageOrPrintOptions.EmfRenderSetting property

Paramètre pour le rendu des métafichiers Emf dans le fichier source.

```csharp
public EmfRenderSetting EmfRenderSetting { get; set; }
```

### Remarques

Les métafichiers EMF identifiés comme "EMF+ Dual" peuvent contenir à la fois des enregistrements EMF+ et des enregistrements EMF. Chaque type d'enregistrement peut être utilisé pour rendre l'image, uniquement les enregistrements EMF+, ou uniquement les enregistrements EMF. Lorsque EmfPlusPrefer est défini, les enregistrements EMF+ seront analysés lors du rendu de l'image, sinon seuls les enregistrements EMF seront analysés. La valeur par défaut est EmfOnly. Pour les frameworks qui dépendent de .NET System.Drawing.Common, ce paramètre est ignoré.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing; // Added missing namespace AsposeCellsExamples
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyEmfRenderSettingDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur avec du contenu de test
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "EMF Rendering Setting Test";
            worksheet.Cells["C5"].Value = "Sample Content for Image Rendering";

            // Créer des options de rendu d'image
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Tiff;
            options.TiffCompression = TiffCompression.CompressionLZW;

            // Afficher le paramètre actuel
            Console.WriteLine("Default EmfRenderSetting: " + options.EmfRenderSetting);

            // Rendre avec les paramètres EMF par défaut
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "DefaultEmfSetting.tiff");

            // Modifier le paramètre de rendu EMF et rendre à nouveau
            options.EmfRenderSetting = EmfRenderSetting.EmfPlusPrefer;
            Console.WriteLine("\nModified EmfRenderSetting: " + options.EmfRenderSetting);

            SheetRender modifiedRenderer = new SheetRender(worksheet, options);
            modifiedRenderer.ToImage(0, "ModifiedEmfSetting.tiff");

            Console.WriteLine("\nGenerated TIFF images demonstrating EMF rendering settings.");
        }
    }
}
```

### Voir aussi

* enum [EmfRenderSetting](../../../aspose.cells/emfrendersetting/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


