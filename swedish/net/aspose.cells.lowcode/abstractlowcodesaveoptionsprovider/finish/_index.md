---
title: "AbstractLowCodeSaveOptionsProvider.Finish"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AbstractLowCodeSaveOptionsProvider metod. Frigör resurser efter bearbetning av den aktuella delade delen"
type: docs
url: /sv/net/aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/
---
## AbstractLowCodeSaveOptionsProvider.Finish method

Frigör resurser efter bearbetning av den aktuella delade delen.

```csharp
public virtual void Finish(LowCodeSaveOptions part)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| del | LowCodeSaveOptions | sparaalternativen som används för den aktuella delade delen. |

### Anmärkningar

Som standard stänger den här metoden bara strömmen som anges av [`OutputStream`](../../lowcodesaveoptions/outputstream/) direkt (om sparaalternativen specificerade en Stream som destination). Användaren kan skriva över den här metoden för att styra hur resurser frigörs enligt deras krav och implementeringen av [`GetSaveOptions`](../getsaveoptions/).

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeSaveOptionsProviderMethodFinishWithLowCodeSaveOptionsDemo
    {
        public static void Run()
        {

            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            loadOptions.InputFile = "split.xlsx";

            // Skapa konkret leverantörsinstans
            var provider = new CustomLowCodeSaveOptionsProvider();

            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
            splitOptions.SaveOptionsProvider = provider;
            splitOptions.LoadOptions = loadOptions;

            SpreadsheetSplitter.Process(splitOptions);
                     
          
        }
    }

    // Konkret implementation av AbstractLowCodeSaveOptionsProvider
    public class CustomLowCodeSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override void Finish(LowCodeSaveOptions part)
        { 
            base.Finish(part);
        }
        // Implementera den erforderliga abstrakta metoden
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

### Se även

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [AbstractLowCodeSaveOptionsProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


