---
title: "DocxSaveOptions.AsFlatOpc"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DocxSaveOptions-Eigenschaft. Gibt an, ob als flache OPC-Datei gespeichert wird, die mit dem Open XML SDK erzeugt werden kann"
type: docs
url: /de/net/aspose.cells/docxsaveoptions/asflatopc/
---
## DocxSaveOptions.AsFlatOpc property

Gibt an, ob als flache OPC‑Datei gespeichert wird, die mit dem Open XML SDK erzeugt werden kann

```csharp
public bool AsFlatOpc { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DocxSaveOptionsPropertyAsFlatOpcDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greifen Sie auf das erste Arbeitsblatt zu und fügen Sie Beispieldaten hinzu
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Flat OPC Demo";

            try
            {
                // DocxSaveOptions initialisieren
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // Standardwert der AsFlatOpc-Eigenschaft anzeigen
                Console.WriteLine("Default AsFlatOpc value: " + saveOptions.AsFlatOpc);

                // Setzen Sie AsFlatOpc auf true, um die Verwendung zu demonstrieren
                saveOptions.AsFlatOpc = true;
                Console.WriteLine("AsFlatOpc set to: " + saveOptions.AsFlatOpc);

                // Speichern Sie die Arbeitsmappe als DOCX mit den konfigurierten Optionen
                workbook.Save("AsFlatOpcDemo.docx", saveOptions);
                Console.WriteLine("Document saved successfully with AsFlatOpc option.");
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


