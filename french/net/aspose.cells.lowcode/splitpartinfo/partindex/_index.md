---
title: "SplitPartInfo.PartIndex"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SplitPartInfo. Index de la partie actuelle dans la séquence basée sur 0. 1 signifie qu'il n'y a pas de multiples parties, donc le résultat est unique."
type: docs
url: /fr/net/aspose.cells.lowcode/splitpartinfo/partindex/
---
## SplitPartInfo.PartIndex property

Index de la partie actuelle dans la séquence (base 0). -1 signifie qu'il n'y a pas de parties multiples, donc le résultat est unique.

```csharp
public int PartIndex { get; }
```

### Remarques

Si plusieurs feuilles doivent être traitées et chaque feuille est traitée (divisée) séparément, l'index de partie commence toujours à 0 pour chaque feuille. Par exemple, lors de la conversion d'un classeur en images, il représente l'index de la page de sortie de la feuille actuellement traitée. Et -1 indique qu'il n'y a qu'une seule page pour la feuille actuelle.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SplitPartInfoPropertyPartIndexDemo
    {
        public static void Run()
        {
            try
            {
                // Créer un classeur avec plusieurs feuilles
                Workbook workbook = new Workbook();
                workbook.Worksheets.Add("Sheet1");
                workbook.Worksheets.Add("Sheet2");
                workbook.Worksheets.Add("Sheet3");

                // Enregistrer le classeur pour l'utiliser avec l'opération de division
                workbook.Save("sample.xlsx");

                // Créer des options de chargement
                LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
                loadOptions.InputFile = "sample.xlsx";

                // Créer des options de division avec un fournisseur personnalisé
                LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
                splitOptions.LoadOptions = loadOptions;
                splitOptions.SaveOptionsProvider = new CustomPartIndexProvider();

                // Traiter l'opération de division
                SpreadsheetSplitter.Process(splitOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CustomPartIndexProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            // Démontrer la lecture de la propriété PartIndex
            Console.WriteLine($"Current part PartIndex: {partInfo.PartIndex}");
            Console.WriteLine($"Current part SheetIndex: {partInfo.SheetIndex}");
            Console.WriteLine($"Current part SheetName: {partInfo.SheetName}");

            LowCodeSaveOptions options = new LowCodeSaveOptions();
            options.SaveFormat = SaveFormat.Xlsx;
            options.OutputFile = $"Part_{partInfo.PartIndex}_{partInfo.SheetName}.xlsx";
            return options;
        }
    }
}
```

### Voir aussi

* class [SplitPartInfo](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


