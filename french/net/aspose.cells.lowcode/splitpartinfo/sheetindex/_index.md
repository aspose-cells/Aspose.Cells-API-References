---
title: "SplitPartInfo.SheetIndex"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SplitPartInfo. Index de la feuille où se trouve la partie actuelle. 1 indique qu'il n'y a qu'une seule feuille"
type: docs
url: /fr/net/aspose.cells.lowcode/splitpartinfo/sheetindex/
---
## SplitPartInfo.SheetIndex property

Index de la feuille contenant la partie actuelle. -1 indique qu'il n'y a qu'une seule feuille.

```csharp
public int SheetIndex { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SplitPartInfoPropertySheetIndexDemo
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
                splitOptions.SaveOptionsProvider = new CustomSheetIndexProvider();

                // Traiter l'opération de division
                SpreadsheetSplitter.Process(splitOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CustomSheetIndexProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            // Démontrer la lecture de la propriété SheetIndex
            Console.WriteLine($"Current part SheetIndex: {partInfo.SheetIndex}");
            Console.WriteLine($"Current part SheetName: {partInfo.SheetName}");
            Console.WriteLine($"Current part PartIndex: {partInfo.PartIndex}");

            LowCodeSaveOptions options = new LowCodeSaveOptions();
            options.SaveFormat = SaveFormat.Xlsx;
            options.OutputFile = $"Sheet_{partInfo.SheetIndex}_{partInfo.SheetName}.xlsx";
            return options;
        }
    }
}
```

### Voir aussi

* class [SplitPartInfo](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


