---
title: "DocxSaveOptions.SaveAsEditableShaps"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DocxSaveOptions-Eigenschaft. Speichere alle Zeichenobjekte als editierbare Formen in der Word-Datei. So kannst du sie in Word bearbeiten."
type: docs
url: /de/net/aspose.cells/docxsaveoptions/saveaseditableshaps/
---
## DocxSaveOptions.SaveAsEditableShaps property

Speichere alle Zeichenobjekte als editierbare Formen in der Word-Datei. So kannst du sie in Word bearbeiten.

```csharp
[Obsolete("Use SaveFormat.SaveAsEditableShapes instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool SaveAsEditableShaps { get; set; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Stattdessen bitte die [`SaveAsEditableShapes`](../saveaseditableshapes/)‑Eigenschaft verwenden. Diese Eigenschaft wird 6 Monate nach Mai 2025 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocxSaveOptionsPropertySaveAsEditableShapsDemo
    {
        public static void Run()
        {
            // Erstelle ein Workbook-Objekt und öffne die Excel-Vorlagendatei.
            Workbook workbook = new Workbook("example.xlsx");

            // DocxSaveOptions initialisieren
            DocxSaveOptions saveOptions = new DocxSaveOptions();
            
            // Setze die SaveAsEditableShaps-Eigenschaft auf true.
            saveOptions.SaveAsEditableShaps = true;

            // Speichere das Workbook als DOCX mit den angegebenen Optionen.
            workbook.Save("example.docx", saveOptions);
        }
    }
}
```

### Siehe auch

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


