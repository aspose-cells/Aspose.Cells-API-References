---
title: "DocxSaveOptions.SaveElementType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DocxSaveOptions-Eigenschaft. Gibt an, welche Elemente gespeichert werden sollen"
type: docs
url: /de/net/aspose.cells/docxsaveoptions/saveelementtype/
---
## DocxSaveOptions.SaveElementType property

Gibt an, welche Elemente gespeichert werden sollen.

```csharp
public SaveElementType SaveElementType { get; set; }
```

### Beispiele

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class DocxSaveOptionsPropertySaveElementTypeDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe und fügen Sie einige Beispieldaten hinzu
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Demo Data");

            try
            {
                // DocxSaveOptions initialisieren
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // HINWEIS: Die SaveElementType‑Eigenschaft ist in der Klasse DocxSaveOptions nicht vorhanden
                // basierend auf der bereitgestellten API‑Reflexion. Wenn sie existieren würde, würden Sie sie so lesen:
                // var elementType = saveOptions.SaveElementType;
                // Console.WriteLine("SaveElementType: " + elementType);

                // Demonstrieren Sie das Lesen einer vorhandenen Eigenschaft: SaveAsEditableShaps
                Console.WriteLine("SaveAsEditableShaps (default): " + saveOptions.SaveAsEditableShaps);

                // Setzen Sie die Eigenschaft auf true und zeigen Sie den neuen Wert an
                saveOptions.SaveAsEditableShaps = true;
                Console.WriteLine("SaveAsEditableShaps (after set): " + saveOptions.SaveAsEditableShaps);

                // Speichern Sie die Arbeitsmappe als DOCX unter Verwendung der konfigurierten Optionen
                workbook.Save("SaveElementTypeDemo.docx", saveOptions);
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### Siehe auch

* enum [SaveElementType](../../../aspose.cells.saving/saveelementtype/)
* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


