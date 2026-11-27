---
title: "FileFormatUtil.SaveFormatToExtension"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FileFormatUtil‑metod. Konverterar ett enumererat sparaformatvärde till en filändelse"
type: docs
url: /sv/net/aspose.cells/fileformatutil/saveformattoextension/
---
## FileFormatUtil.SaveFormatToExtension method

Konverterar ett SaveFormat‑enumererat värde till en filändelse.

```csharp
public static string SaveFormatToExtension(SaveFormat format)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| format | SaveFormat | Sparaformatet. |

### Returvärde

Den returnerade filändelsen är en gemenerad sträng med en inledande punkt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodSaveFormatToExtensionWithSaveFormatDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test content");

            // Demonstrera SaveFormatToExtension med olika format
            SaveOptions[] saveOptions = {
                new PdfSaveOptions(),
                new XlsSaveOptions(SaveFormat.Excel97To2003),
                new OoxmlSaveOptions(SaveFormat.Xlsx),
                new OdsSaveOptions()
            };

            foreach (var options in saveOptions)
            {
                string extension = FileFormatUtil.SaveFormatToExtension(options.SaveFormat);
                Console.WriteLine($"SaveFormat: {options.SaveFormat} -> Extension: {extension}");
                
                // Spara med den upptäckta filändelsen
                string fileName = $"output{extension}";
                workbook.Save(fileName, options);
                Console.WriteLine($"Saved file: {fileName}");
            }

            workbook.Dispose();
        }
    }
}
```

### Se även

* enum [SaveFormat](../../saveformat/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


