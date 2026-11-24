---
title: "SplitPartInfo.PartIndex"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SplitPartInfo Eigenschaft. Index des aktuellen Teils in einer nullbasierten Sequenz. 1 bedeutet, dass es keine mehreren Teile gibt, sodass das Ergebnis ein einzelnes ist."
type: docs
url: /de/net/aspose.cells.lowcode/splitpartinfo/partindex/
---
## SplitPartInfo.PartIndex property

Index des aktuellen Teils in der Sequenz (0‑basiert). -1 bedeutet, dass es keine mehreren Teile gibt, sodass das Ergebnis ein einzelner ist.

```csharp
public int PartIndex { get; }
```

### Hinweise

Wenn mehrere Blätter verarbeitet werden müssen und jedes Blatt separat (gesplittet) verarbeitet wird, beginnt der Teilindex für jedes Blatt immer bei 0. Zum Beispiel, beim Konvertieren einer Arbeitsmappe in Bilder, stellt er den Ausgabeseitenindex des aktuell verarbeiteten Blatts dar. Und -1 bedeutet, dass es für das aktuelle Blatt nur eine Seite gibt.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SplitPartInfoPropertyPartIndexDemo
    {
        public static void Run()
        {
            try
            {
                // Erstelle eine Arbeitsmappe mit mehreren Blättern
                Workbook workbook = new Workbook();
                workbook.Worksheets.Add("Sheet1");
                workbook.Worksheets.Add("Sheet2");
                workbook.Worksheets.Add("Sheet3");

                // Speichere die Arbeitsmappe zur Verwendung mit der Split-Operation
                workbook.Save("sample.xlsx");

                // Ladeoptionen erstellen
                LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
                loadOptions.InputFile = "sample.xlsx";

                // Erstelle Split-Optionen mit benutzerdefiniertem Anbieter
                LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
                splitOptions.LoadOptions = loadOptions;
                splitOptions.SaveOptionsProvider = new CustomPartIndexProvider();

                // Den Split‑Vorgang verarbeiten
                SpreadsheetSplitter.Process(splitOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CustomPartIndexProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            // Demonstriere das Auslesen der PartIndex-Eigenschaft
            Console.WriteLine($"Current part PartIndex: {partInfo.PartIndex}");
            Console.WriteLine($"Current part SheetIndex: {partInfo.SheetIndex}");
            Console.WriteLine($"Current part SheetName: {partInfo.SheetName}");

            LowCodeSaveOptions options = new LowCodeSaveOptions();
            options.SaveFormat = SaveFormat.Xlsx;
            options.OutputFile = $"Part_{partInfo.PartIndex}_{partInfo.SheetName}.xlsx";
            return options;
        }
    }
}
```

### Siehe auch

* class [SplitPartInfo](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


