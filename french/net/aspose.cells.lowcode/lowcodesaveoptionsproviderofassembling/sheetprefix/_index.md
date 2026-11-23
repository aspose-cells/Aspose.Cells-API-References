---
title: "LowCodeSaveOptionsProviderOfAssembling.SheetPrefix"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LowCodeSaveOptionsProviderOfAssembling. Préfixe pour l'index de la feuille de calcul"
type: docs
url: /fr/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/sheetprefix/
---
## LowCodeSaveOptionsProviderOfAssembling.SheetPrefix property

Préfixe pour l’index de la feuille de calcul.

```csharp
public string SheetPrefix { get; set; }
```

### Remarques

S'il n'y a qu'une seule feuille de calcul et que [`BuildPathWithSheetAlways`](../buildpathwithsheetalways/) est faux, alors ce préfixe et l'index (ou le nom) de la feuille ne seront pas ajoutés au chemin de fichier résultant.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertySheetPrefixDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            LowCodeSaveOptionsProviderOfAssembling provider = new LowCodeSaveOptionsProviderOfAssembling();
            provider.PathHeader = "output/";
            provider.PathTail = ".xlsx";
            provider.UseSheetName = false;

            Console.WriteLine("Current SheetPrefix: " + provider.SheetPrefix);
            
            provider.SheetPrefix = "Report_";
            Console.WriteLine("New SheetPrefix: " + provider.SheetPrefix);

            for (int sheetIndex = 0; sheetIndex < workbook.Worksheets.Count; sheetIndex++)
            {
                string fileName = $"{provider.PathHeader}{provider.SheetPrefix}{sheetIndex}{provider.PathTail}";
                Console.WriteLine($"Generated file path: {fileName}");
            }

            provider.SheetPrefix = "Data_";
            Console.WriteLine("Updated SheetPrefix: " + provider.SheetPrefix);

            for (int sheetIndex = 0; sheetIndex < workbook.Worksheets.Count; sheetIndex++)
            {
                string fileName = $"{provider.PathHeader}{provider.SheetPrefix}{sheetIndex}{provider.PathTail}";
                Console.WriteLine($"Generated file path: {fileName}");
            }
        }
    }
}
```

### Voir aussi

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


