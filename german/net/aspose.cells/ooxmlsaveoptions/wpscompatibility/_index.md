---
title: "OoxmlSaveOptions.WpsCompatibility"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OoxmlSaveOptions-Eigenschaft. Gibt an, ob die xls-Datei stärker mit WPS kompatibel gemacht werden soll"
type: docs
url: /de/net/aspose.cells/ooxmlsaveoptions/wpscompatibility/
---
## OoxmlSaveOptions.WpsCompatibility property

Gibt an, ob die XLS-Datei stärker mit WPS kompatibel gemacht werden soll.

```csharp
[Obsolete("Use WorkbookSetting.WpsCompatibility property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool WpsCompatibility { get; set; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die WorkbookSetting.WpsCompatibility‑Eigenschaft. Diese Methode wird 12 Monate nach Dezember 2025 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OoxmlSaveOptionsPropertyWpsCompatibilityDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu und füge Beispieldaten hinzu
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test WPS Compatibility");
            
            // Erstellen Sie OOXML-Speicheroptionen und aktivieren Sie die WPS-Kompatibilität
            OoxmlSaveOptions options = new OoxmlSaveOptions();
            options.WpsCompatibility = true;
            
            // Speichern Sie die Arbeitsmappe mit WPS-Kompatibilität
            workbook.Save("output_with_wps_compatibility.xlsx", options);
            
            Console.WriteLine("Workbook saved with WPS compatibility enabled.");
        }
    }
}
```

### Siehe auch

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


