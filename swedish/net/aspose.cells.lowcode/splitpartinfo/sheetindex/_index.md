---
title: "SplitPartInfo.SheetIndex"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SplitPartInfo-egenskap. Index för bladet där den aktuella delen finns. 1 betyder att det bara finns ett blad"
type: docs
url: /sv/net/aspose.cells.lowcode/splitpartinfo/sheetindex/
---
## SplitPartInfo.SheetIndex property

Index för bladet där den aktuella delen finns. -1 indikerar att det bara finns ett blad.

```csharp
public int SheetIndex { get; }
```

### Exempel

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
                // Skapa en arbetsbok med flera blad
                Workbook workbook = new Workbook();
                workbook.Worksheets.Add("Sheet1");
                workbook.Worksheets.Add("Sheet2");
                workbook.Worksheets.Add("Sheet3");

                // Spara arbetsboken för att använda i delningsoperationen
                workbook.Save("sample.xlsx");

                // Skapa laddningsalternativ
                LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
                loadOptions.InputFile = "sample.xlsx";

                // Skapa delningsalternativ med anpassad leverantör
                LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
                splitOptions.LoadOptions = loadOptions;
                splitOptions.SaveOptionsProvider = new CustomSheetIndexProvider();

                // Bearbeta delningsoperationen
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

            // Demonstrera läsning av SheetIndex‑egenskapen
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

### Se även

* class [SplitPartInfo](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


