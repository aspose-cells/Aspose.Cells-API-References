---
title: "Classe SplitPartInfo"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.LowCode.SplitPartInfo. Représente les informations d'une entrée/sortie pour plusieurs entrées/sorties, comme la page actuelle à rendre lors de la conversion d'une feuille de calcul en image"
type: docs
url: /fr/net/aspose.cells.lowcode/splitpartinfo/
---
## SplitPartInfo class

Représente les informations d'une entrée/sortie pour plusieurs entrées/sorties, comme la page actuelle à rendre lors de la conversion d'une feuille de calcul en image.

```csharp
public class SplitPartInfo
```

## Propriétés

| Nom | Description |
| --- | --- |
| [PartIndex](../../aspose.cells.lowcode/splitpartinfo/partindex/) { get; } | Index de la partie actuelle dans la séquence (base 0). -1 signifie qu'il n'y a pas de parties multiples, donc le résultat est unique. |
| [SheetIndex](../../aspose.cells.lowcode/splitpartinfo/sheetindex/) { get; } | Index de la feuille contenant la partie actuelle. -1 indique qu'il n'y a qu'une seule feuille. |
| [SheetName](../../aspose.cells.lowcode/splitpartinfo/sheetname/) { get; } | Nom de la feuille contenant la partie actuelle. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassSplitPartInfoDemo
    {
        public static void Run()
        {
            try
            {
                // Créer un classeur avec plusieurs feuilles à des fins de démonstration
                Workbook workbook = new Workbook();
                workbook.Worksheets.Add("Sheet1");
                workbook.Worksheets.Add("Sheet2");
                workbook.Worksheets.Add("Sheet3");

                // Créer LowCodeLoadOptions et LowCodeSplitOptions
                LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
                loadOptions.InputFile = "sample.xlsx";

                LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
                splitOptions.LoadOptions = loadOptions;

                // Créer un fournisseur personnalisé pour démontrer l'utilisation de SplitPartInfo
                splitOptions.SaveOptionsProvider = new CustomSplitOptionsProvider();

                // Traiter l'opération de division
                SpreadsheetSplitter.Process(splitOptions);

                Console.WriteLine("Split operation completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CustomSplitOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            // Démontrer l'accès aux propriétés de SplitPartInfo
            Console.WriteLine($"Processing part: Index={partInfo.PartIndex}, SheetIndex={partInfo.SheetIndex}, SheetName={partInfo.SheetName}");

            LowCodeSaveOptions options = new LowCodeSaveOptions();
            options.SaveFormat = SaveFormat.Xlsx;
            options.OutputFile = $"Part_{partInfo.PartIndex}_{partInfo.SheetName}.xlsx";
            return options;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


