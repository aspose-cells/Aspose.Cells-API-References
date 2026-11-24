---
title: "HtmlSaveOptions.ExportWorksheetProperties"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions property. Gibt an, ob Arbeitsblatt‑Eigenschaften exportiert werden. Der Standardwert ist true. Wenn Sie die HTML‑ oder MHT‑Datei nach Excel importieren möchten, behalten Sie bitte den Standardwert bei."
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/exportworksheetproperties/
---
## HtmlSaveOptions.ExportWorksheetProperties property

Gibt an, ob Arbeitsblatt‑Eigenschaften exportiert werden. Der Standardwert ist true. Wenn Sie die HTML‑ oder MHT‑Datei nach Excel importieren möchten, behalten Sie bitte den Standardwert bei.

```csharp
public bool ExportWorksheetProperties { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportWorksheetPropertiesDemo
    {
        public static void Run()
        {
            // Erstelle eine Beispielarbeitsmappe mit Testdaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Data");

            // Setze HTML‑Speicheroptionen mit deaktiviertem ExportWorksheetProperties
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportWorksheetProperties = false;
            
            // Speichern mit deaktivierten Arbeitsblatt‑Eigenschaften
            workbook.Save("output_without_worksheet_props.html", options);

            // Aktiviere den Export von Arbeitsblatt‑Eigenschaften
            options.ExportWorksheetProperties = true;
            
            // Speichern mit aktivierten Arbeitsblatt-Eigenschaften
            workbook.Save("output_with_worksheet_props.html", options);
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


