---
title: "LowCodeSaveOptionsProviderOfAssembling.SplitPartIndexOffset"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LowCodeSaveOptionsProviderOfAssembling Eigenschaft. Offset des Indexes der geteilten Teile zwischen dem im Dateipfad verwendeten Wert und seinem tatsächlichen Wert PartIndex"
type: docs
url: /de/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/splitpartindexoffset/
---
## LowCodeSaveOptionsProviderOfAssembling.SplitPartIndexOffset property

Offset des Indexes des geteilten Teils zwischen dem im Dateipfad verwendeten Wert und seinem tatsächlichen Wert ([`PartIndex`](../../splitpartinfo/partindex/)).

```csharp
public int SplitPartIndexOffset { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertySplitPartIndexOffsetDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe mit Testdaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Arbeitsblatt befüllen, um mehrere geteilte Teile zu erstellen
            for(int i = 0; i < 150; i++)
            {
                worksheet.Cells[$"A{i+1}"].Value = $"Item {i+1}";
            }

            // Seitenumbrüche konfigurieren, um in 3 Teile zu teilen
            worksheet.HorizontalPageBreaks.Add(0, 50);
            worksheet.HorizontalPageBreaks.Add(0, 100);

            // Provider erstellen und Save-Options konfigurieren
            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "output/Part_",
                SplitPartPrefix = "-",
                PathTail = ".xlsx",
                SplitPartIndexOffset = 10
            };

            // Zeige die anfängliche Konfiguration
            Console.WriteLine($"Initial SplitPartIndexOffset: {provider.SplitPartIndexOffset}");
            Console.WriteLine("First save operation (offset 10):");
            Console.WriteLine($"Expected filenames: output/Part_-10.xlsx, output/Part_-11.xlsx, output/Part_-12.xlsx");

            // Offset ändern und neue Konfiguration anzeigen
            provider.SplitPartIndexOffset = 0;
            Console.WriteLine($"\nModified SplitPartIndexOffset: {provider.SplitPartIndexOffset}");
            Console.WriteLine("Second save operation (offset 0):");
            Console.WriteLine($"Expected filenames: output/Part_-0.xlsx, output/Part_-1.xlsx, output/Part_-2.xlsx");

            // Der eigentliche Speicherungsvorgang wäre typischerweise:
            // workbook.Save("output/main.xlsx", new OoxmlSaveOptions { SaveProvider = provider });
        }
    }
}
```

### Siehe auch

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


