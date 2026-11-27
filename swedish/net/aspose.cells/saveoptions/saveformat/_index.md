---
title: "SaveOptions.SaveFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SaveOptions-egenskap. Hämtar filformatet för sparning"
type: docs
url: /sv/net/aspose.cells/saveoptions/saveformat/
---
## SaveOptions.SaveFormat property

Hämtar formatet för sparad fil.

```csharp
public SaveFormat SaveFormat { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertySaveFormatDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");

            // Demonstrera olika sparformat
            SaveOptions[] options = {
                new PdfSaveOptions(),
                new OoxmlSaveOptions(),
                new HtmlSaveOptions()
            };

            foreach (var saveOptions in options)
            {
                string extension = FileFormatUtil.SaveFormatToExtension(saveOptions.SaveFormat);
                Console.WriteLine($"Saving as {saveOptions.SaveFormat} with extension: {extension}");

                string outputPath = $"output_{Guid.NewGuid().ToString("N").Substring(0, 8)}{extension}";
                workbook.Save(outputPath, saveOptions);
                Console.WriteLine($"Saved to: {outputPath}");
            }

            // Rensa upp
            workbook.Dispose();
        }
    }
}
```

### Se även

* enum [SaveFormat](../../saveformat/)
* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


