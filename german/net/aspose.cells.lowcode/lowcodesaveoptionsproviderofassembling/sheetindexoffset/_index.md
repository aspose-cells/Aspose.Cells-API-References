---
title: "LowCodeSaveOptionsProviderOfAssembling.SheetIndexOffset"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LowCodeSaveOptionsProviderOfAssembling‑Eigenschaft. Offset des Blatt‑Index zwischen dem im Dateipfad verwendeten Wert und dem tatsächlichen Wert SheetIndex"
type: docs
url: /de/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/sheetindexoffset/
---
## LowCodeSaveOptionsProviderOfAssembling.SheetIndexOffset property

Offset des Blatt‑Index zwischen dem im Dateipfad verwendeten Wert und dem tatsächlichen Wert ([`SheetIndex`](../../splitpartinfo/sheetindex/)).

```csharp
public int SheetIndexOffset { get; set; }
```

### Hinweise

Wirkt nur, wenn [`UseSheetName`](../usesheetname/) false ist.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertySheetIndexOffsetDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe mit mehreren Arbeitsblättern
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("SalesData");
            workbook.Worksheets.Add("Inventory");

            // Speicheroptionen‑Anbieter initialisieren
            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "output/Quarter_",
                PathTail = ".xlsx",
                SheetPrefix = "Sheet",
                SheetIndexOffset = 10,
                SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Xlsx }
            };

            // Ursprünglichen Offset anzeigen
            Console.WriteLine($"Original SheetIndexOffset: {provider.SheetIndexOffset}");

            // Speichern mit ursprünglichem Offset (Blätter werden mit 10 und 11 nummeriert)
            workbook.Save("output/with_offset", provider.SaveOptionsTemplate.SaveFormat);

            // Offset ändern und erneut speichern
            provider.SheetIndexOffset = 100;
            Console.WriteLine($"Modified SheetIndexOffset: {provider.SheetIndexOffset}");
            
            // Speichern mit neuem Offset (Blätter werden mit 100 und 101 nummeriert)
            workbook.Save("output/with_modified_offset", provider.SaveOptionsTemplate.SaveFormat);
        }
    }
}
```

### Siehe auch

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


