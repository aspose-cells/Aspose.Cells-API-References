---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.BuildPathWithSheetAlways"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LowCodeSaveOptionsProviderOfPlaceHolders Eigenschaft. Ob der Blatt-Index oder -Name immer zum Dateipfad hinzugefügt wird. Standardwert ist false, das heißt, wenn es nur ein Blatt gibt, werden der Blatt-Index und -Name sowie das entsprechende PräfixSheetNamePrefix nicht zum Dateipfad hinzugefügt."
type: docs
url: /de/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/buildpathwithsheetalways/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.BuildPathWithSheetAlways property

Ob der Blatt-Index oder -Name immer zum Dateipfad hinzugefügt wird. Standardwert ist false, das heißt, wenn es nur ein Blatt gibt, werden der Blatt-Index und -Name sowie das entsprechende Präfix([`SheetNamePrefix`](../sheetnameprefix/)) nicht zum Dateipfad hinzugefügt.

```csharp
public bool BuildPathWithSheetAlways { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertyBuildPathWithSheetAlwaysDemo
    {
        public static void Run()
        {
            // Arbeitsmappe mit zwei Blättern erstellen, um Pfadunterschiede zu demonstrieren.
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Provider mit Blatt-Index-Platzhalter konfigurieren.
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("Output_{sheet_index}.xlsx")
            {
                // Blatt-Index-Offset demonstrieren (optional).
                SheetIndexOffset = 1
            };

            Console.WriteLine($"Initial BuildPathWithSheetAlways: {provider.BuildPathWithSheetAlways}");

            // Speichern mit Blatt-Index nur bei mehreren Blättern (Standardverhalten).
            provider.BuildPathWithSheetAlways = false;
            SaveWithProvider(workbook, provider, "DefaultBehavior");

            // Blatt-Index in Dateinamen erzwingen, selbst bei einzelnen Blättern.
            provider.BuildPathWithSheetAlways = true;
            Console.WriteLine($"Modified BuildPathWithSheetAlways: {provider.BuildPathWithSheetAlways}");
            SaveWithProvider(workbook, provider, "ForcedSheetIndex");
        }

        private static void SaveWithProvider(Workbook workbook, LowCodeSaveOptionsProviderOfPlaceHolders provider, string saveDescription)
        {
            // Speicheroptionen mit JSON-Format konfigurieren, um das Aufteilen zu ermöglichen.
            var saveOptions = new LowCodeSaveOptions
            {
                SaveFormat = SaveFormat.Json
            };

            // Provider mit den Speicheroptionen konfigurieren
            provider.SaveOptionsTemplate = saveOptions;

            // Speichern mit vom Provider bestimmten Pfaden
            Console.WriteLine($"Saving with {saveDescription} - check output files");
            workbook.Save($"dummy_{saveDescription}.json", saveOptions.SaveFormat);
        }
    }
}
```

### Siehe auch

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


