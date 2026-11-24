---
title: "DocxSaveOptions.SaveAsEditableShapes"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DocxSaveOptions‑Eigenschaft. Speichert alle Zeichenobjekte als editierbare Formen in der Word‑Datei, sodass Sie sie in Word bearbeiten können"
type: docs
url: /de/net/aspose.cells/docxsaveoptions/saveaseditableshapes/
---
## DocxSaveOptions.SaveAsEditableShapes property

Alle Zeichenobjekte als bearbeitbare Formen in der Word‑Datei speichern, sodass Sie sie in Word bearbeiten können.

```csharp
public bool SaveAsEditableShapes { get; set; }
```

### Hinweise

Nur für Diagramme.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DocxSaveOptionsPropertySaveAsEditableShapesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greifen Sie auf das erste Arbeitsblatt zu und fügen Sie Beispieldaten hinzu
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Editable Shapes Demo";

            try
            {
                // DocxSaveOptions initialisieren
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // Zeigen Sie den Standardwert der Eigenschaft SaveAsEditableShapes an
                Console.WriteLine("Default SaveAsEditableShapes value: " + saveOptions.SaveAsEditableShapes);

                // Setzen Sie SaveAsEditableShapes auf true, um die Verwendung zu demonstrieren
                saveOptions.SaveAsEditableShapes = true;
                Console.WriteLine("SaveAsEditableShapes set to: " + saveOptions.SaveAsEditableShapes);

                // Speichern Sie die Arbeitsmappe als DOCX mit den konfigurierten Optionen
                workbook.Save("SaveAsEditableShapesDemo.docx", saveOptions);
                Console.WriteLine("Document saved successfully with SaveAsEditableShapes option.");
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


