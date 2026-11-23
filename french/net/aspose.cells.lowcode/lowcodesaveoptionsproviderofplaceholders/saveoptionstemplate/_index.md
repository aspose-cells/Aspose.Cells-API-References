---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.SaveOptionsTemplate"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LowCodeSaveOptionsProviderOfPlaceHolders. Le modèle pour créer une instance d'options d'enregistrement dans GetSaveOptions"
type: docs
url: /fr/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/saveoptionstemplate/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.SaveOptionsTemplate property

Le modèle pour créer une instance d'options d'enregistrement dans [`GetSaveOptions`](../getsaveoptions/).

```csharp
public LowCodeSaveOptions SaveOptionsTemplate { get; set; }
```

### Remarques

Si le modèle a été spécifié, alors l'instance créée copiera tous les paramètres depuis celui-ci et mettra à jour le fichier de sortie en conséquence.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertySaveOptionsTemplateDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            
            // Initialiser le fournisseur avec un modèle de chemin contenant des espaces réservés
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("output/Sheet_{sheet}_Part_{part}.pdf");
            
            // Afficher l'état initial du modèle
            Console.WriteLine($"Initial SaveOptionsTemplate: {(provider.SaveOptionsTemplate == null ? "Not set" : "Configured")}");
            
            // Créer et configurer un nouveau modèle d'options d'enregistrement
            provider.SaveOptionsTemplate = new LowCodePdfSaveOptions
            {
                PdfOptions = new PdfSaveOptions  // Fixed property name from PdfSaveOptions to PdfOptions
                {
                    Compliance = PdfCompliance.PdfA1a,
                    ExportDocumentStructure = true
                }
            };

            // Configurer les paramètres de division
            provider.BuildPathWithSheetAlways = true;
            provider.SplitPartPrefix = "Split_";
            
            // Afficher les options PDF configurées
            var pdfOptions = (LowCodePdfSaveOptions)provider.SaveOptionsTemplate;
            Console.WriteLine($"Configured PDF Compliance: {pdfOptions.PdfOptions.Compliance}");  // Fixed property access
            Console.WriteLine($"Document Structure Export: {pdfOptions.PdfOptions.ExportDocumentStructure}");  // Fixed property access

            // Ajouter un saut de page pour créer des parties découpées
            worksheet.HorizontalPageBreaks.Add(0);
            
            // Enregistrer en utilisant la configuration du fournisseur (la division/enregistrement réelle aurait lieu ici)
            Console.WriteLine("Workbook prepared with SaveOptionsTemplate configuration");
        }
    }
}
```

### Voir aussi

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


