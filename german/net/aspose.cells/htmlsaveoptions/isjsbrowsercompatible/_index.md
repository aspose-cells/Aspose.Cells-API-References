---
title: "HtmlSaveOptions.IsJsBrowserCompatible"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Gibt an, ob JavaScript mit Browsern kompatibel ist, die JavaScript nicht unterstützen. Der Standardwert ist true"
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/isjsbrowsercompatible/
---
## HtmlSaveOptions.IsJsBrowserCompatible property

Gibt an, ob JavaScript mit Browsern kompatibel ist, die kein JavaScript unterstützen. Der Standardwert ist true.

```csharp
public bool IsJsBrowserCompatible { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsJsBrowserCompatibleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test JavaScript Compatibility");

            // Konfigurieren Sie die HTML-Speicheroptionen mit IsJsBrowserCompatible auf true gesetzt
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                IsJsBrowserCompatible = true,
                ExportFormula = true,
                PresentationPreference = true
            };

            // Speichern Sie die Arbeitsmappe mit JavaScript-Kompatibilität
            workbook.Save("JsCompatibleOutput.html", saveOptions);

            Console.WriteLine("HTML file with JavaScript compatibility saved successfully.");
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


