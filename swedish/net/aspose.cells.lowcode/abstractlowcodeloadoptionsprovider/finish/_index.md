---
title: "AbstractLowCodeLoadOptionsProvider.Finish"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AbstractLowCodeLoadOptionsProvider-metod. Frigör resurser efter bearbetning av den aktuella delen av indata"
type: docs
url: /sv/net/aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/finish/
---
## AbstractLowCodeLoadOptionsProvider.Finish method

Frigör resurser efter att ha bearbetat den aktuella delen av indata.

```csharp
public virtual void Finish(LowCodeLoadOptions part)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| del | LowCodeLoadOptions | laddningsalternativen som används för den aktuella delade delen. |

### Anmärkningar

Som standard stänger den här metoden bara strömmen som anges av [`InputStream`](../../lowcodeloadoptions/inputstream/) direkt (om laddningsalternativen specificerade en Ström som källa). Användaren kan skriva över den här metoden för att kontrollera hur resurser frigörs enligt deras krav och implementeringen av [`Current`](../current/).

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.Collections;

    public class AbstractLowCodeLoadOptionsProviderMethodFinishWithLowCodeLoadOptionsDemo
    {
        public static void Run()
        {
            string[] files = { "file1.xlsx", "file2.xlsx", "file3.xlsx" };

            CustomLoadOptionsProvider provider = new CustomLoadOptionsProvider(files);

            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
            saveOptions.OutputFile = "result.xlsx";
            saveOptions.SaveFormat = SaveFormat.Xlsx;

            LowCodeMergeOptions mergeOptions = new LowCodeMergeOptions();
            mergeOptions.LoadOptionsProvider = provider;
            mergeOptions.SaveOptions = saveOptions;

            SpreadsheetMerger.Process(mergeOptions);
        }
    }

    public class CustomLoadOptionsProvider : AbstractLowCodeLoadOptionsProvider
    {       

        public IEnumerator fileIter;
        public CustomLoadOptionsProvider(string[] files)
        {
            fileIter = files.GetEnumerator();
            current = new LowCodeLoadOptions();
        }
        private LowCodeLoadOptions current;

        public override LowCodeLoadOptions Current => current;

        public override bool MoveNext()
        {
            if (fileIter.MoveNext())
            {
                current = new LowCodeLoadOptions();
                current.InputFile = fileIter.Current.ToString();
                return true;
            }
            
            return false;
        }

        public override void Finish(LowCodeLoadOptions part)
        {
            base.Finish(part);
        }
    }
}
```

### Se även

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [AbstractLowCodeLoadOptionsProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


