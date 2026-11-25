---
title: "SplitPartInfo.SheetName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SplitPartInfo. Nome del foglio in cui si trova la parte corrente"
type: docs
url: /it/net/aspose.cells.lowcode/splitpartinfo/sheetname/
---
## SplitPartInfo.SheetName property

Nome del foglio in cui si trova la parte corrente.

```csharp
public string SheetName { get; }
```

### Osservazioni

Può essere null in alcune situazioni, ad esempio durante il rendering dell'intera cartella di lavoro in immagine TIFF.

### Esempi

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

            // Crea un'istanza concreta del provider
            var provider = new CustomLowCodeSaveOptionsProvider();

            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
            splitOptions.SaveOptionsProvider = provider;
            splitOptions.LoadOptions = loadOptions;

            SpreadsheetSplitter.Process(splitOptions);
        }
    }

    // Implementazione concreta di AbstractLowCodeSaveOptionsProvider
    public class CustomLowCodeSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override void Finish(LowCodeSaveOptions part)
        {
            base.Finish(part);
        }
        // Implementa il metodo astratto richiesto
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

### Vedi anche

* class [SplitPartInfo](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


