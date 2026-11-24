---
title: "Klasse SplitPartInfo"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.LowCode.SplitPartInfo Klasse. Stellt die Informationen eines Eingabe/Ausgabe-Paares für mehrere Eingaben/Ausgaben dar, wie z. B. die aktuelle Seite, die beim Konvertieren einer Tabelle in ein Bild gerendert wird."
type: docs
url: /de/net/aspose.cells.lowcode/splitpartinfo/
---
## SplitPartInfo class

Stellt die Informationen eines Eingabe-/Ausgabe-Elements für mehrere Eingaben/Ausgaben dar, z. B. die aktuelle Seite, die beim Konvertieren einer Tabelle in ein Bild gerendert werden soll.

```csharp
public class SplitPartInfo
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [PartIndex](../../aspose.cells.lowcode/splitpartinfo/partindex/) { get; } | Index des aktuellen Teils in der Sequenz (0‑basiert). -1 bedeutet, dass es keine mehreren Teile gibt, sodass das Ergebnis ein einzelner ist. |
| [SheetIndex](../../aspose.cells.lowcode/splitpartinfo/sheetindex/) { get; } | Index des Blatts, in dem sich der aktuelle Teil befindet. -1 bedeutet, dass es nur ein Blatt gibt. |
| [SheetName](../../aspose.cells.lowcode/splitpartinfo/sheetname/) { get; } | Name des Blatts, in dem sich der aktuelle Teil befindet. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassSplitPartInfoDemo
    {
        public static void Run()
        {
            try
            {
                // Erstelle eine Arbeitsmappe mit mehreren Blättern für die Demonstration
                Workbook workbook = new Workbook();
                workbook.Worksheets.Add("Sheet1");
                workbook.Worksheets.Add("Sheet2");
                workbook.Worksheets.Add("Sheet3");

                // LowCodeLoadOptions und LowCodeSplitOptions erstellen
                LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
                loadOptions.InputFile = "sample.xlsx";

                LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
                splitOptions.LoadOptions = loadOptions;

                // Einen benutzerdefinierten Provider erstellen, um die Verwendung von SplitPartInfo zu demonstrieren
                splitOptions.SaveOptionsProvider = new CustomSplitOptionsProvider();

                // Den Split‑Vorgang verarbeiten
                SpreadsheetSplitter.Process(splitOptions);

                Console.WriteLine("Split operation completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CustomSplitOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            // Demonstrieren, wie auf SplitPartInfo‑Eigenschaften zugegriffen wird
            Console.WriteLine($"Processing part: Index={partInfo.PartIndex}, SheetIndex={partInfo.SheetIndex}, SheetName={partInfo.SheetName}");

            LowCodeSaveOptions options = new LowCodeSaveOptions();
            options.SaveFormat = SaveFormat.Xlsx;
            options.OutputFile = $"Part_{partInfo.PartIndex}_{partInfo.SheetName}.xlsx";
            return options;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


