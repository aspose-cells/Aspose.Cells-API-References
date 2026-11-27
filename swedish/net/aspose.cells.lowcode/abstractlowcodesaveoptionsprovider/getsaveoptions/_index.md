---
title: "AbstractLowCodeSaveOptionsProvider.GetSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AbstractLowCodeSaveOptionsProvider metod. Hämtar sparaalternativen från vilka utdatainställningarna för den aktuella delade delen ska tas. Att returnera null betyder att hoppa över den givna delen."
type: docs
url: /sv/net/aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/getsaveoptions/
---
## AbstractLowCodeSaveOptionsProvider.GetSaveOptions method

Hämtar sparalternativen från vilka utdatainställningarna för den aktuella delade delen hämtas. Att returnera null betyder att hoppa över den angivna delen.

```csharp
public abstract LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
```

### Exempel

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

            // Skapa konkret leverantörsinstans
            var provider = new CustomSaveOptionsProvider();

            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
            splitOptions.SaveOptionsProvider = provider;
            splitOptions.LoadOptions = loadOptions;

            SpreadsheetSplitter.Process(splitOptions);
        }
    }

    // Anpassad implementation av AbstractLowCodeSaveOptionsProvider
    public class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            // Skapa anpassade sparaalternativ baserat på delinformation
            LowCodeSaveOptions result = new LowCodeSaveOptions();
            result.SaveFormat = SaveFormat.Xlsx;
            result.OutputFile = $"Part_{partInfo.PartIndex}_Sheet_{partInfo.SheetName}.xlsx";
            Console.WriteLine(result.OutputFile);
            return result;

        }
    }
}
```

### Se även

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [SplitPartInfo](../../splitpartinfo/)
* class [AbstractLowCodeSaveOptionsProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


