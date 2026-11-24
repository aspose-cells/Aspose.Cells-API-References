---
title: "LowCodeSplitOptions.SaveOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LowCodeSplitOptions-Eigenschaft. Speicheroptionen zum Speichern der geteilten Teile"
type: docs
url: /de/net/aspose.cells.lowcode/lowcodesplitoptions/saveoptions/
---
## LowCodeSplitOptions.SaveOptions property

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

    public class LowCodeSplitOptionsPropertySaveOptionsDemo
    {
        public static void Run()
        {
            // Neue Arbeitsmappe erstellen und Beispieldaten hinzufügen
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");

            // Erstellen Sie eine Instanz von LowCodeSplitOptions
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();

            // Anfänglichen SaveOptions-Wert anzeigen (standardmäßig null)
            Console.WriteLine("Initial SaveOptions value: " + (splitOptions.SaveOptions == null ? "null" : splitOptions.SaveOptions.ToString()));

            // LowCodeSaveOptions für das PDF-Format erstellen und konfigurieren
            LowCodeSaveOptions pdfSaveOptions = new LowCodeSaveOptions();
            pdfSaveOptions.SaveFormat = SaveFormat.Pdf;

            // Die Speicheroptionen den SplitOptions zuweisen
            splitOptions.SaveOptions = pdfSaveOptions;

            // Aktualisierten SaveOptions-Wert anzeigen
            Console.WriteLine("Updated SaveOptions SaveFormat: " + splitOptions.SaveOptions.SaveFormat);

            // Beispiel für ein Anwendungsszenario: Das Aufteilen der Arbeitsmappe würde die Teile als PDF speichern
            // (Der tatsächliche Aufteilungscode würde von der Implementierung der Aspose.Cells.LowCode API abhängen)
            // LowCodeEngine.Split(workbook, splitOptions, "output_directory/");
            
            // Speichern Sie die ursprüngliche Arbeitsmappe zur Demonstration (nicht von SplitOptions beeinflusst)
            workbook.Save("LowCodeSplitOptionsPropertySaveOptionsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [LowCodeSplitOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


