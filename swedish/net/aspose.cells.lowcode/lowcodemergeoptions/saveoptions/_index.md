---
title: "LowCodeMergeOptions.SaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LowCodeMergeOptions-egenskap. Sparalternativ för att spara de delade delarna"
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodemergeoptions/saveoptions/
---
## LowCodeMergeOptions.SaveOptions property

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

    public class LowCodeMergeOptionsPropertySaveOptionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Merged Data");

            // Initiera sammanslagningsalternativ
            LowCodeMergeOptions mergeOptions = new LowCodeMergeOptions();
            Console.WriteLine("Initial SaveOptions: " + (mergeOptions.SaveOptions?.GetType().Name ?? "null"));

            // Konfigurera nya sparalternativ
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
            saveOptions.SaveFormat = SaveFormat.Xlsx;
            // Ange lösenord via arbetsbokinställningar
            workbook.Settings.Password = "Aspose1234!";
            mergeOptions.SaveOptions = saveOptions;

            // Visa effekten genom att spara med konfigurerade alternativ
            workbook.Save("MergedWithOptions.xlsx", saveOptions.SaveFormat);

            Console.WriteLine("Workbook saved with password-protected SaveOptions.");
        }
    }
}
```

### Se även

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [LowCodeMergeOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


