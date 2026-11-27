---
title: "Klass SplitPartInfo"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.LowCode.SplitPartInfo-klass. Representerar informationen för en in-/utdata för flera in-/utdata, såsom aktuell sida som ska renderas vid konvertering av kalkylblad till bild"
type: docs
url: /sv/net/aspose.cells.lowcode/splitpartinfo/
---
## SplitPartInfo class

Representerar informationen för en in-/utdata för flera in-/utdata, såsom aktuell sida som ska renderas vid konvertering av kalkylblad till bild.

```csharp
public class SplitPartInfo
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [PartIndex](../../aspose.cells.lowcode/splitpartinfo/partindex/) { get; } | Index för aktuell del i sekvensen (0-baserad). -1 betyder att det inte finns flera delar så resultatet är enstaka. |
| [SheetIndex](../../aspose.cells.lowcode/splitpartinfo/sheetindex/) { get; } | Index för bladet där den aktuella delen finns. -1 indikerar att det bara finns ett blad. |
| [SheetName](../../aspose.cells.lowcode/splitpartinfo/sheetname/) { get; } | Namn på bladet där den aktuella delen finns. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassSplitPartInfoDemo
    {
        public static void Run()
        {
            try
            {
                // Skapa en arbetsbok med flera blad för demonstration
                Workbook workbook = new Workbook();
                workbook.Worksheets.Add("Sheet1");
                workbook.Worksheets.Add("Sheet2");
                workbook.Worksheets.Add("Sheet3");

                // Skapa LowCodeLoadOptions och LowCodeSplitOptions
                LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
                loadOptions.InputFile = "sample.xlsx";

                LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
                splitOptions.LoadOptions = loadOptions;

                // Skapa en anpassad leverantör för att demonstrera användning av SplitPartInfo
                splitOptions.SaveOptionsProvider = new CustomSplitOptionsProvider();

                // Bearbeta delningsoperationen
                SpreadsheetSplitter.Process(splitOptions);

                Console.WriteLine("Split operation completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CustomSplitOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            // Demonstrera åtkomst till SplitPartInfo-egenskaper
            Console.WriteLine($"Processing part: Index={partInfo.PartIndex}, SheetIndex={partInfo.SheetIndex}, SheetName={partInfo.SheetName}");

            LowCodeSaveOptions options = new LowCodeSaveOptions();
            options.SaveFormat = SaveFormat.Xlsx;
            options.OutputFile = $"Part_{partInfo.PartIndex}_{partInfo.SheetName}.xlsx";
            return options;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


