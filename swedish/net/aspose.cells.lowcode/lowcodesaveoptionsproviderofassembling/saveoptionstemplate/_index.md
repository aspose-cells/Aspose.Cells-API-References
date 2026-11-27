---
title: "LowCodeSaveOptionsProviderOfAssembling.SaveOptionsTemplate"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LowCodeSaveOptionsProviderOfAssembling egenskap. Mallen för att skapa en instans av sparalternativ i GetSaveOptions"
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/saveoptionstemplate/
---
## LowCodeSaveOptionsProviderOfAssembling.SaveOptionsTemplate property

Mallen för att skapa en instans av sparalternativ i [`GetSaveOptions`](../getsaveoptions/).

```csharp
public LowCodeSaveOptions SaveOptionsTemplate { get; set; }
```

### Anmärkningar

Om mallen har angetts kommer den skapade instansen att kopiera alla inställningar från den och uppdatera utdatafilen i enlighet med detta.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Saving;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertySaveOptionsTemplateDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med två kalkylblad
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            Worksheet worksheet1 = workbook.Worksheets[0];
            Worksheet worksheet2 = workbook.Worksheets[1];
            worksheet1.Cells["A1"].PutValue("Sheet1 Content");
            worksheet2.Cells["A1"].PutValue("Sheet2 Content");

            // Skapa en instans av LowCodeSaveOptionsProviderOfAssembling
            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "Output/Sheet",
                PathTail = ".xlsx",
                BuildPathWithSheetAlways = true,
                UseSheetName = false
            };

            // Visa det initiala tillståndet för SaveOptionsTemplate
            Console.WriteLine("Initial SaveOptionsTemplate is " + (provider.SaveOptionsTemplate == null ? "null" : "set"));

            // Konfigurera SaveOptionsTemplate med kryptering
            provider.SaveOptionsTemplate = new LowCodeSaveOptions();
            Console.WriteLine("SaveOptionsTemplate configured");

            // Skapa LowCode-sparalternativ
            var saveOptions = new LowCodeSaveOptions();

            // Spara arbetsboken med den konfigurerade leverantören (kommer att generera separata filer per blad)
            workbook.Save("output_combined.xlsx", saveOptions.SaveFormat);

            Console.WriteLine("Demo executed successfully. Check output files.");
        }
    }
}
```

### Se även

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


