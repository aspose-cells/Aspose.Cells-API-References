---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.SheetIndexPrefix"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LowCodeSaveOptionsProviderOfPlaceHolders Eigenschaft. Präfix für den Index des Arbeitsblatts"
type: docs
url: /de/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetindexprefix/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.SheetIndexPrefix property

Präfix für den Index des Arbeitsblatts.

```csharp
public string SheetIndexPrefix { get; set; }
```

### Hinweise

Wenn es nur ein Arbeitsblatt gibt und [`BuildPathWithSheetAlways`](../buildpathwithsheetalways/) false ist, dann werden dieses Präfix und der Blattindex (oder Name) nicht zum resultierenden Dateipfad hinzugefügt.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertySheetIndexPrefixDemo
    {
        public static void Run()
        {
            // Eine neue Arbeitsmappe mit mehreren Arbeitsblättern erstellen
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Instanz von LowCodeSaveOptionsProviderOfPlaceHolders erstellen
            string pathTemplate = "output_{sheetindex}.xlsx";
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders(pathTemplate);

            // Zeige SheetIndexPrefix an und ändere es.
            Console.WriteLine("Original SheetIndexPrefix: " + provider.SheetIndexPrefix);
            provider.SheetIndexPrefix = "sheet_";
            Console.WriteLine("Modified SheetIndexPrefix: " + provider.SheetIndexPrefix);

            // Weitere erforderliche Eigenschaften festlegen
            provider.BuildPathWithSheetAlways = true;
            provider.SaveOptionsTemplate = new LowCodeSaveOptions();

            // Demonstriere die Auswirkung von SheetIndexPrefix auf Dateipfade.
            foreach (Worksheet sheet in workbook.Worksheets)
            {
                // Da wir SplitPartInfo nicht direkt erstellen und befüllen können,
                // Wir werden einfach das Namensmuster ohne sie demonstrieren.
                Console.WriteLine($"Sheet {sheet.Name} would save to: output_{provider.SheetIndexPrefix}{sheet.Index}.xlsx");
            }

            // Speichere die Arbeitsmappe, um das Namensmuster zu demonstrieren.
            workbook.Save("output_sheet_0.xlsx");
        }
    }
}
```

### Siehe auch

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


