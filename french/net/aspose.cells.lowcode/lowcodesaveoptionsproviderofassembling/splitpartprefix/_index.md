---
title: "LowCodeSaveOptionsProviderOfAssembling.SplitPartPrefix"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LowCodeSaveOptionsProviderOfAssembling. Préfixe pour l'index de la partie découpée"
type: docs
url: /fr/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/splitpartprefix/
---
## LowCodeSaveOptionsProviderOfAssembling.SplitPartPrefix property

Préfixe pour l’index de la partie découpée.

```csharp
public string SplitPartPrefix { get; set; }
```

### Remarques

S'il n'y a qu'une seule partie découpée et que [`BuildPathWithSplitPartAlways`](../buildpathwithsplitpartalways/) est false, alors ce préfixe et l'index de la partie découpée (0) ne seront pas ajoutés au chemin du fichier résultant.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertySplitPartPrefixDemo
    {
        public static void Run()
        {
            // Créer un classeur avec des données s'étendant sur plusieurs pages
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 100; i++)
                worksheet.Cells[$"A{i + 1}"].Value = $"Data Row {i + 1}";

            // Configurer les paramètres de page pour créer plusieurs pages
            worksheet.PageSetup.PrintArea = "A1:A30";
            worksheet.PageSetup.FitToPagesTall = 1;

            // Initialiser le fournisseur d'options d'enregistrement avec la configuration de division
            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "SplitResults/",
                SplitPartPrefix = "OriginalPart_",
                PathTail = ".pdf",
                SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Pdf }
            };

            Console.WriteLine($"Initial SplitPartPrefix: {provider.SplitPartPrefix}");

            // Enregistrer avec le préfixe initial (générera SplitResults/OriginalPart_0.pdf etc.)
            workbook.Save("InitialSplit.pdf", new PdfSaveOptions());

            // Modifier le préfixe de division
            provider.SplitPartPrefix = "ModifiedPart_";
            Console.WriteLine($"Updated SplitPartPrefix: {provider.SplitPartPrefix}");

            // Enregistrer avec le préfixe modifié (générera SplitResults/ModifiedPart_0.pdf etc.)
            workbook.Save("ModifiedSplit.pdf", new PdfSaveOptions());
        }
    }
}
```

### Voir aussi

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


