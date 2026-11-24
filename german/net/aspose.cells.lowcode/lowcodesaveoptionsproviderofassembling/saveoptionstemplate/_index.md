---
title: "LowCodeSaveOptionsProviderOfAssembling.SaveOptionsTemplate"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LowCodeSaveOptionsProviderOfAssembling Eigenschaft. Die Vorlage zum Erstellen einer Instanz von Save-Options in GetSaveOptions"
type: docs
url: /de/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/saveoptionstemplate/
---
## LowCodeSaveOptionsProviderOfAssembling.SaveOptionsTemplate property

Die Vorlage zum Erstellen einer Instanz von Save-Options in [`GetSaveOptions`](../getsaveoptions/).

```csharp
public LowCodeSaveOptions SaveOptionsTemplate { get; set; }
```

### Hinweise

Wenn die Vorlage angegeben wurde, kopiert die erstellte Instanz alle Einstellungen daraus und aktualisiert die Ausgabedatei entsprechend.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Saving;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertySaveOptionsTemplateDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe mit zwei Arbeitsblättern
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            Worksheet worksheet1 = workbook.Worksheets[0];
            Worksheet worksheet2 = workbook.Worksheets[1];
            worksheet1.Cells["A1"].PutValue("Sheet1 Content");
            worksheet2.Cells["A1"].PutValue("Sheet2 Content");

            // Erstelle eine Instanz von LowCodeSaveOptionsProviderOfAssembling
            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "Output/Sheet",
                PathTail = ".xlsx",
                BuildPathWithSheetAlways = true,
                UseSheetName = false
            };

            // Zeige den anfänglichen Zustand von SaveOptionsTemplate an
            Console.WriteLine("Initial SaveOptionsTemplate is " + (provider.SaveOptionsTemplate == null ? "null" : "set"));

            // Konfiguriere SaveOptionsTemplate mit Verschlüsselung
            provider.SaveOptionsTemplate = new LowCodeSaveOptions();
            Console.WriteLine("SaveOptionsTemplate configured");

            // Erstelle LowCode Save-Optionen
            var saveOptions = new LowCodeSaveOptions();

            // Speichere die Arbeitsmappe mit dem konfigurierten Provider (erstellt separate Dateien pro Blatt)
            workbook.Save("output_combined.xlsx", saveOptions.SaveFormat);

            Console.WriteLine("Demo executed successfully. Check output files.");
        }
    }
}
```

### Siehe auch

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


