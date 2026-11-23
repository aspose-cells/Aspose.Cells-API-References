---
title: "LowCodeImageSaveOptions.SaveOptionsProvider"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LowCodeImageSaveOptions. Fournisseur d'options d'enregistrement pour enregistrer les images générées"
type: docs
url: /fr/net/aspose.cells.lowcode/lowcodeimagesaveoptions/saveoptionsprovider/
---
## LowCodeImageSaveOptions.SaveOptionsProvider property

Fournisseur d’options d’enregistrement pour enregistrer les images générées.

```csharp
public AbstractLowCodeSaveOptionsProvider SaveOptionsProvider { get; set; }
```

### Remarques

La sortie([`OutputFile`](../../lowcodesaveoptions/outputfile/) ou [`OutputStream`](../../lowcodesaveoptions/outputstream/)) spécifiée par cette instance n'aura aucun effet lorsque cette propriété est définie. Au lieu de cela, la sortie de chaque image générée sera spécifiée par le fournisseur.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeImageSaveOptionsPropertySaveOptionsProviderDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Sample Image Data");
            
            // Créez une instance de LowCodeImageSaveOptions
            LowCodeImageSaveOptions saveOptions = new LowCodeImageSaveOptions();
            saveOptions.SaveFormat = SaveFormat.Png;
            saveOptions.ImageOptions = new ImageOrPrintOptions();
            
            // Créer un SaveOptionsProvider personnalisé
            CustomSaveOptionsProvider provider = new CustomSaveOptionsProvider();
            saveOptions.SaveOptionsProvider = provider;
            
            // Affichez le SaveOptionsProvider actuel
            Console.WriteLine("Current SaveOptionsProvider: " + (saveOptions.SaveOptionsProvider != null ? "Custom Provider" : "null"));
            
            // Démontrez l'effet en enregistrant avec différentes options
            workbook.Save("output_with_provider.png", saveOptions.SaveFormat);
            
            // Changez pour un fournisseur nul
            saveOptions.SaveOptionsProvider = null;
            Console.WriteLine("Changed SaveOptionsProvider to: " + (saveOptions.SaveOptionsProvider != null ? "Custom Provider" : "null"));
            
            workbook.Save("output_without_provider.png", saveOptions.SaveFormat);
        }
    }

    public class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
        {
            // Retournez des options d'enregistrement personnalisées pour chaque partie
            return new LowCodeImageSaveOptions()
            {
                SaveFormat = SaveFormat.Jpg,  // Changed from Jpeg to Jpg
                ImageOptions = new ImageOrPrintOptions()
                {
                    Quality = 90,
                    HorizontalResolution = 300,
                    VerticalResolution = 300
                }
            };
        }

        public override void Finish(LowCodeSaveOptions part)
        {
            // Effectuez tout nettoyage après l'enregistrement
            Console.WriteLine("Finished saving part with custom options");
        }
    }
}
```

### Voir aussi

* class [AbstractLowCodeSaveOptionsProvider](../../abstractlowcodesaveoptionsprovider/)
* class [LowCodeImageSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


