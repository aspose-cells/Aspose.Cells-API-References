---
title: "SplitPartInfo.PartIndex"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SplitPartInfo-egenskap. Index för den aktuella delen i sekvensen, 0‑baserad. 1 betyder att det inte finns flera delar så resultatet är enstaka."
type: docs
url: /sv/net/aspose.cells.lowcode/splitpartinfo/partindex/
---
## SplitPartInfo.PartIndex property

Index för aktuell del i sekvensen (0-baserad). -1 betyder att det inte finns flera delar så resultatet är enstaka.

```csharp
public int PartIndex { get; }
```

### Anmärkningar

Om flera blad måste bearbetas och varje blad bearbetas (delas) separat, startar delindex alltid från 0 för varje blad. Till exempel, när en arbetsbok konverteras till bilder, representerar det utdata sidindex för det blad som för närvarande bearbetas. Och -1 betyder att det bara finns en sida för det aktuella bladet.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SplitPartInfoPropertyPartIndexDemo
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
                splitOptions.SaveOptionsProvider = new CustomPartIndexProvider();

                // Bearbeta delningsoperationen
                SpreadsheetSplitter.Process(splitOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CustomPartIndexProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            // Demonstrera läsning av PartIndex‑egenskapen
            Console.WriteLine($"Current part PartIndex: {partInfo.PartIndex}");
            Console.WriteLine($"Current part SheetIndex: {partInfo.SheetIndex}");
            Console.WriteLine($"Current part SheetName: {partInfo.SheetName}");

            LowCodeSaveOptions options = new LowCodeSaveOptions();
            options.SaveFormat = SaveFormat.Xlsx;
            options.OutputFile = $"Part_{partInfo.PartIndex}_{partInfo.SheetName}.xlsx";
            return options;
        }
    }
}
```

### Se även

* class [SplitPartInfo](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


