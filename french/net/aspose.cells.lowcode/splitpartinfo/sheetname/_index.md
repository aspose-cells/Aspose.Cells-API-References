---
title: "SplitPartInfo.SheetName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SplitPartInfo. Nom de la feuille où se trouve la partie actuelle"
type: docs
url: /fr/net/aspose.cells.lowcode/splitpartinfo/sheetname/
---
## SplitPartInfo.SheetName property

Nom de la feuille contenant la partie actuelle.

```csharp
public string SheetName { get; }
```

### Remarques

Peut être nul dans certaines situations, comme lors du rendu du classeur complet en image TIFF.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using AsposeCellsExamples.AbstractLowCodeSaveOptionsProviderMethodFinishWithLowCodeSaveOptionsDemo;
    using System;
    using System.Reflection;

    public class SplitPartInfoPropertySheetNameDemo
    {
        public static void Run()
        {
            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            loadOptions.InputFile = "split.xlsx";

            // Créez une instance concrète du fournisseur
            var provider = new CustomLowCodeSaveOptionsProvider();

            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
            splitOptions.SaveOptionsProvider = provider;
            splitOptions.LoadOptions = loadOptions;

            SpreadsheetSplitter.Process(splitOptions);
        }
    }

    // Implémentation concrète de AbstractLowCodeSaveOptionsProvider
    public class CustomLowCodeSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override void Finish(LowCodeSaveOptions part)
        {
            base.Finish(part);
        }
        // Implémentez la méthode abstraite requise
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            LowCodeSaveOptions result = new LowCodeSaveOptions();
            result.SaveFormat = SaveFormat.Xlsx;
            result.OutputFile = partInfo.SheetName + "_split.xlsx";
            Console.WriteLine(result.OutputFile);
            return result;
        }
    }
}
```

### Voir aussi

* class [SplitPartInfo](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


