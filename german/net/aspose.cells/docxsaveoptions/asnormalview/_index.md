---
title: "DocxSaveOptions.AsNormalView"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DocxSaveOptions-Eigenschaft. Exportieren einer Excel-Datei in eine docx-Datei als Normalansicht. Wenn diese Eigenschaft true ist, wird ein Bereich ausgegeben und keine Skalierung wirkt. Der Standardwert ist false."
type: docs
url: /de/net/aspose.cells/docxsaveoptions/asnormalview/
---
## DocxSaveOptions.AsNormalView property

Exportieren einer Excel‑Datei in eine docx‑Datei als Normalansicht. Wenn diese Eigenschaft true ist, wird ein Bereich ausgegeben und keine Skalierung wirkt. Der Standardwert ist false.

```csharp
public bool AsNormalView { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DocxSaveOptionsPropertyAsNormalViewDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greifen Sie auf das erste Arbeitsblatt zu und fügen Sie Beispieldaten hinzu
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Normal View Demo";

            try
            {
                // DocxSaveOptions initialisieren
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // Zeige den Standardwert der AsNormalView-Eigenschaft an.
                Console.WriteLine("Default AsNormalView value: " + saveOptions.AsNormalView);

                // Setze AsNormalView auf true, um die Verwendung zu demonstrieren.
                saveOptions.AsNormalView = true;
                Console.WriteLine("AsNormalView set to: " + saveOptions.AsNormalView);

                // Speichern Sie die Arbeitsmappe als DOCX mit den konfigurierten Optionen
                workbook.Save("AsNormalViewDemo.docx", saveOptions);
                Console.WriteLine("Document saved successfully with AsNormalView option.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


