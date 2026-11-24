---
title: "PaginatedSaveOptions.CheckFontCompatibility"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PaginatedSaveOptions-Eigenschaft. Gibt an, ob die Schriftkompatibilität für jedes Zeichen im Text überprüft werden soll"
type: docs
url: /de/net/aspose.cells/paginatedsaveoptions/checkfontcompatibility/
---
## PaginatedSaveOptions.CheckFontCompatibility property

Gibt an, ob die Schriftkompatibilität für jedes Zeichen im Text überprüft werden soll.

```csharp
public bool CheckFontCompatibility { get; set; }
```

### Hinweise

Der Standardwert ist true. Das Deaktivieren dieser Eigenschaft kann zu besserer Leistung führen. Aber wenn die Standard‑ oder angegebene Schriftart des Textes/Zeichens nicht zum Rendern verwendet werden kann, können im erzeugten PDF unlesbare Zeichen (wie Blockzeichen) auftreten. In einer solchen Situation sollte der Benutzer diese Eigenschaft auf true belassen, damit eine alternative Schriftart gesucht und zum Rendern des Textes verwendet werden kann;

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyCheckFontCompatibilityDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Font Compatibility Test");

            // Paginierten Speicheroptionen erstellen
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // CheckFontCompatibility-Eigenschaft demonstrieren
            saveOptions.CheckFontCompatibility = false; // Disable font compatibility checking
            
            // Weitere erforderliche Eigenschaften festlegen
            saveOptions.DefaultFont = "Arial";
            saveOptions.CheckWorkbookDefaultFont = true;

            // Dokument mit den angegebenen Optionen speichern
            workbook.Save("PaginatedSaveOptions_CheckFontCompatibility.pdf", saveOptions);
            
            Console.WriteLine("Document saved with CheckFontCompatibility = false");
        }
    }
}
```

### Siehe auch

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


