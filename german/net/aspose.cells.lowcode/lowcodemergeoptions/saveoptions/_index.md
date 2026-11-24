---
title: "LowCodeMergeOptions.SaveOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LowCodeMergeOptions-Eigenschaft. Speicheroptionen zum Speichern der geteilten Teile"
type: docs
url: /de/net/aspose.cells.lowcode/lowcodemergeoptions/saveoptions/
---
## LowCodeMergeOptions.SaveOptions property

Speicheroptionen zum Speichern der geteilten Teile.

```csharp
public LowCodeSaveOptions SaveOptions { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeMergeOptionsPropertySaveOptionsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Merged Data");

            // Initialisiere Merge-Optionen
            LowCodeMergeOptions mergeOptions = new LowCodeMergeOptions();
            Console.WriteLine("Initial SaveOptions: " + (mergeOptions.SaveOptions?.GetType().Name ?? "null"));

            // Konfiguriere neue Speicheroptionen
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
            saveOptions.SaveFormat = SaveFormat.Xlsx;
            // Passwort über Arbeitsmappen-Einstellungen festlegen
            workbook.Settings.Password = "Aspose1234!";
            mergeOptions.SaveOptions = saveOptions;

            // Demonstriere die Wirkung, indem du mit konfigurierten Optionen speicherst
            workbook.Save("MergedWithOptions.xlsx", saveOptions.SaveFormat);

            Console.WriteLine("Workbook saved with password-protected SaveOptions.");
        }
    }
}
```

### Siehe auch

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [LowCodeMergeOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


