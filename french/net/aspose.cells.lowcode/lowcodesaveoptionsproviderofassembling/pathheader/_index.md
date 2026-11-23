---
title: "LowCodeSaveOptionsProviderOfAssembling.PathHeader"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "LowCodeSaveOptionsProviderOfAssembling property. En-tête avant le contenu ajouté de la feuille et la partie fractionnée du chemin du fichier"
type: docs
url: /fr/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/pathheader/
---
## LowCodeSaveOptionsProviderOfAssembling.PathHeader property

Partie d’en‑tête (avant le contenu ajouté de la feuille et de la partie découpée) du chemin du fichier.

```csharp
public string PathHeader { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertyPathHeaderDemo
    {
        public static void Run()
        {
            // Créer un classeur avec des données qui seront divisées en plusieurs parties
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 150; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data row {i + 1}";
            }

            // Initialiser le fournisseur d'options d'enregistrement avec les valeurs par défaut
            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "output/QuarterlyReport_",
                PathTail = ".html",
                UseSheetName = true,
                SaveOptionsTemplate = new LowCodeSaveOptions() // Changed from HtmlSaveOptions to LowCodeSaveOptions
            };

            Console.WriteLine($"Initial PathHeader: {provider.PathHeader}");

            // Modifier la configuration du chemin
            provider.PathHeader = "output/ModifiedReport_";
            provider.SheetPrefix = "Sheet_";
            provider.SplitPartPrefix = "Part_";

            // Démontrer l'effet en enregistrant avec la configuration actuelle du fournisseur
            workbook.Save("result.html", SaveFormat.Html); // Changed second parameter to SaveFormat.Html

            Console.WriteLine("Check 'output' directory for split files named like 'ModifiedReport_Sheet_0_Part_0.html'");
        }
    }
}
```

### Voir aussi

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


