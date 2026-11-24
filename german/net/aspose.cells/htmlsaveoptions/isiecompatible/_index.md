---
title: "HtmlSaveOptions.IsIECompatible"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions property. Gibt an, ob das ausgegebene HTML mit dem IE-Browser kompatibel ist. Der Standardwert ist false"
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/isiecompatible/
---
## HtmlSaveOptions.IsIECompatible property

Gibt an, ob das ausgegebene HTML mit dem IE‑Browser kompatibel ist. Der Standardwert ist false.

```csharp
public bool IsIECompatible { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsIECompatibleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("HTML Export Demo");

            // HTML‑Speicheroptionen erstellen
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Setze die IsIECompatible-Eigenschaft
            saveOptions.IsIECompatible = false; // Disable IE compatibility mode
            
            // Speichere die Arbeitsmappe mit HTML-Optionen
            workbook.Save("HtmlExportDemo.html", saveOptions);

            Console.WriteLine("HTML file saved with IsIECompatible = false");
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


