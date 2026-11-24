---
title: "LowCodeSaveOptionsProviderOfAssembling.SplitPartPrefix"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LowCodeSaveOptionsProviderOfAssembling‑Eigenschaft. Präfix für den Index des geteilten Teils"
type: docs
url: /de/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/splitpartprefix/
---
## LowCodeSaveOptionsProviderOfAssembling.SplitPartPrefix property

Präfix für den Index des geteilten Teils.

```csharp
public string SplitPartPrefix { get; set; }
```

### Hinweise

Wenn es nur einen geteilten Teil gibt und [`BuildPathWithSplitPartAlways`](../buildpathwithsplitpartalways/) false ist, werden dieses Präfix und der Index des geteilten Teils (0) nicht zum resultierenden Dateipfad hinzugefügt.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertySplitPartPrefixDemo
    {
        public static void Run()
        {
            // Arbeitsmappe mit Daten über mehrere Seiten erstellen
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 100; i++)
                worksheet.Cells[$"A{i + 1}"].Value = $"Data Row {i + 1}";

            // Konfigurieren Sie die Seiteneinstellungen, um mehrere Seiten zu erstellen
            worksheet.PageSetup.PrintArea = "A1:A30";
            worksheet.PageSetup.FitToPagesTall = 1;

            // Initialisieren Sie den Speicheroptionen‑Provider mit Split‑Konfiguration
            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "SplitResults/",
                SplitPartPrefix = "OriginalPart_",
                PathTail = ".pdf",
                SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Pdf }
            };

            Console.WriteLine($"Initial SplitPartPrefix: {provider.SplitPartPrefix}");

            // Speichern mit dem ursprünglichen Präfix (erzeugt SplitResults/OriginalPart_0.pdf usw.)
            workbook.Save("InitialSplit.pdf", new PdfSaveOptions());

            // Split‑Präfix ändern
            provider.SplitPartPrefix = "ModifiedPart_";
            Console.WriteLine($"Updated SplitPartPrefix: {provider.SplitPartPrefix}");

            // Speichern mit geändertem Präfix (erzeugt SplitResults/ModifiedPart_0.pdf usw.)
            workbook.Save("ModifiedSplit.pdf", new PdfSaveOptions());
        }
    }
}
```

### Siehe auch

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


