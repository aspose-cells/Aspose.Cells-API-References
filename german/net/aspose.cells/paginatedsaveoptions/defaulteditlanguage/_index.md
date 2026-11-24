---
title: "PaginatedSaveOptions.DefaultEditLanguage"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PaginatedSaveOptions-Eigenschaft. Gibt die Standardsprache für die Bearbeitung zurück oder legt sie fest"
type: docs
url: /de/net/aspose.cells/paginatedsaveoptions/defaulteditlanguage/
---
## PaginatedSaveOptions.DefaultEditLanguage property

Liest oder setzt die Standardsprache für die Bearbeitung.

```csharp
public DefaultEditLanguage DefaultEditLanguage { get; set; }
```

### Hinweise

Es kann unterschiedliche Layouts für Textabsätze anzeigen/rendern, wenn verschiedene Bearbeitungssprachen festgelegt sind. Standard ist Auto.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyDefaultEditLanguageDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie etwas CJK-Text hinzu, um die DefaultEditLanguage‑Eigenschaft zu demonstrieren
            worksheet.Cells["A1"].PutValue("日本語のテキスト");
            worksheet.Cells["A2"].PutValue("中文文本");
            worksheet.Cells["A3"].PutValue("한글 텍스트");

            // Erstellen Sie PDF-Speicheroptionen und setzen Sie CJK als Standardsprache für die Bearbeitung
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.DefaultEditLanguage = DefaultEditLanguage.CJK;
            
            // Speichere die Arbeitsmappe mit den angegebenen Optionen
            workbook.Save("output.pdf", pdfSaveOptions);
            
            Console.WriteLine("Workbook saved with CJK as default edit language.");
        }
    }
}
```

### Siehe auch

* enum [DefaultEditLanguage](../../defaulteditlanguage/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


