---
title: "AbstractLowCodeSaveOptionsProvider.GetSaveOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo AbstractLowCodeSaveOptionsProvider. Ottiene le opzioni di salvataggio da cui ricavare le impostazioni di output per la parte attualmente suddivisa. Restituire null indica di saltare la parte specificata."
type: docs
url: /it/net/aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/getsaveoptions/
---
## AbstractLowCodeSaveOptionsProvider.GetSaveOptions method

Ottiene le opzioni di salvataggio da cui ricavare le impostazioni di output per la parte attualmente divisa. Restituire null indica di saltare la parte fornita.

```csharp
public abstract LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using AsposeCellsExamples.AbstractLowCodeSaveOptionsProviderMethodFinishWithLowCodeSaveOptionsDemo;
    using System;

    public class AbstractLowCodeSaveOptionsProviderMethodGetSaveOptionsWithSplitPartInfoDemo
    {
        public static void Run()
        {
            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            loadOptions.InputFile = "split.xlsx";

            // Crea un'istanza concreta del provider
            var provider = new CustomSaveOptionsProvider();

            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
            splitOptions.SaveOptionsProvider = provider;
            splitOptions.LoadOptions = loadOptions;

            SpreadsheetSplitter.Process(splitOptions);
        }
    }

    // Implementazione personalizzata di AbstractLowCodeSaveOptionsProvider
    public class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            // Crea opzioni di salvataggio personalizzate basate sulle informazioni della parte
            LowCodeSaveOptions result = new LowCodeSaveOptions();
            result.SaveFormat = SaveFormat.Xlsx;
            result.OutputFile = $"Part_{partInfo.PartIndex}_Sheet_{partInfo.SheetName}.xlsx";
            Console.WriteLine(result.OutputFile);
            return result;

        }
    }
}
```

### Vedi anche

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [SplitPartInfo](../../splitpartinfo/)
* class [AbstractLowCodeSaveOptionsProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


