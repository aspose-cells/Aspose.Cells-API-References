---
title: "LowCodeSaveOptionsProviderOfAssembling.SheetIndexOffset"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LowCodeSaveOptionsProviderOfAssembling. Décalage de l'index des feuilles entre ce qui est utilisé dans le chemin du fichier et sa valeur réelle SheetIndex"
type: docs
url: /fr/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/sheetindexoffset/
---
## LowCodeSaveOptionsProviderOfAssembling.SheetIndexOffset property

Décalage de l'index de la feuille entre ce qui est utilisé dans le chemin du fichier et sa valeur réelle ([`SheetIndex`](../../splitpartinfo/sheetindex/)).

```csharp
public int SheetIndexOffset { get; set; }
```

### Remarques

Ne prend effet que lorsque [`UseSheetName`](../usesheetname/) est false.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertySheetIndexOffsetDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur avec plusieurs feuilles
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("SalesData");
            workbook.Worksheets.Add("Inventory");

            // Initialiser le fournisseur d'options d'enregistrement
            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "output/Quarter_",
                PathTail = ".xlsx",
                SheetPrefix = "Sheet",
                SheetIndexOffset = 10,
                SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Xlsx }
            };

            // Afficher le décalage original
            Console.WriteLine($"Original SheetIndexOffset: {provider.SheetIndexOffset}");

            // Enregistrer avec le décalage initial (les feuilles seront numérotées 10 et 11)
            workbook.Save("output/with_offset", provider.SaveOptionsTemplate.SaveFormat);

            // Modifier le décalage et enregistrer à nouveau
            provider.SheetIndexOffset = 100;
            Console.WriteLine($"Modified SheetIndexOffset: {provider.SheetIndexOffset}");
            
            // Enregistrer avec le nouveau décalage (les feuilles seront numérotées 100 et 101)
            workbook.Save("output/with_modified_offset", provider.SaveOptionsTemplate.SaveFormat);
        }
    }
}
```

### Voir aussi

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


