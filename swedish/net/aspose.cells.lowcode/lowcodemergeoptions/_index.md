---
title: "Klass LowCodeMergeOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.LowCode.LowCodeMergeOptions class. Alternativ för att slå samman flera mallfiler till en"
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodemergeoptions/
---
## LowCodeMergeOptions class

Alternativ för att slå samman flera mallfiler till en.

```csharp
public class LowCodeMergeOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [LowCodeMergeOptions](lowcodemergeoptions/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [LoadOptionsProvider](../../aspose.cells.lowcode/lowcodemergeoptions/loadoptionsprovider/) { get; set; } | Leverantör av sparaalternativ för att spara de delade delarna. |
| [SaveOptions](../../aspose.cells.lowcode/lowcodemergeoptions/saveoptions/) { get; set; } | Sparaalternativ för att spara de delade delarna. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassLowCodeMergeOptionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Skapa och konfigurera LowCodeMergeOptions
            LowCodeMergeOptions mergeOptions = new LowCodeMergeOptions();
            
            // Ange sparalternativ för utdataformat
            mergeOptions.SaveOptions = new LowCodeSaveOptions();
            
            // Tilldela anpassad leverantör av laddningsalternativ
            mergeOptions.LoadOptionsProvider = new CustomLoadOptionsProvider();
            
            // Exempel på integration (hypotetisk användning med sammanslagningsfunktionalitet)
            // Detta skulle vanligtvis anropas med faktiska filsökvägar
            // Workbook.Merge(new string[] { \"template1.xlsx\", \"template2.xlsx\" }, mergeOptions);
            
            // Spara arbetsboken (demonstrationssyfte)
            workbook.Save("LowCodeMergeOptionsDemo.xlsx");
        }
    }

    // Anpassad leverantör som implementerar abstrakt klass
    public class CustomLoadOptionsProvider : AbstractLowCodeLoadOptionsProvider
    {
        public override bool MoveNext()
        {
            // Minimal implementation för att uppfylla abstrakt krav
            return false;
        }

        public override LowCodeLoadOptions Current
        {
            get { throw new InvalidOperationException(); }
        }

        public LoadOptions GetLoadOptions(string fileName)
        {
            if (fileName.EndsWith(".xlsx", StringComparison.OrdinalIgnoreCase))
            {
                return new LoadOptions(LoadFormat.Xlsx);
            }
            return new LoadOptions();
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


