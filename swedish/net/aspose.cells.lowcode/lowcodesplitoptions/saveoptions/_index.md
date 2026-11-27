---
title: "LowCodeSplitOptions.SaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LowCodeSplitOptions‑egenskap. Sparalternativ för att spara de delade delarna"
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodesplitoptions/saveoptions/
---
## LowCodeSplitOptions.SaveOptions property

Sparaalternativ för att spara de delade delarna.

```csharp
public LowCodeSaveOptions SaveOptions { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSplitOptionsPropertySaveOptionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och lägg till exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");

            // Skapa en instans av LowCodeSplitOptions
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();

            // Visa initialt SaveOptions‑värde (null som standard)
            Console.WriteLine("Initial SaveOptions value: " + (splitOptions.SaveOptions == null ? "null" : splitOptions.SaveOptions.ToString()));

            // Skapa och konfigurera LowCodeSaveOptions för PDF-format
            LowCodeSaveOptions pdfSaveOptions = new LowCodeSaveOptions();
            pdfSaveOptions.SaveFormat = SaveFormat.Pdf;

            // Tilldela sparalternativen till SplitOptions
            splitOptions.SaveOptions = pdfSaveOptions;

            // Visa uppdaterat SaveOptions‑värde
            Console.WriteLine("Updated SaveOptions SaveFormat: " + splitOptions.SaveOptions.SaveFormat);

            // Exempel på användningsscenario: Att dela arbetsboken skulle spara delarna som PDF
            // (Den faktiska delningskoden skulle bero på Aspose.Cells.LowCode API-implementationen)
            // LowCodeEngine.Split(workbook, splitOptions, "output_directory/");
            
            // Spara den ursprungliga arbetsboken för demonstration (påverkas inte av SplitOptions)
            workbook.Save("LowCodeSplitOptionsPropertySaveOptionsDemo.xlsx");
        }
    }
}
```

### Se även

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [LowCodeSplitOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


