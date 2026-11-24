---
title: "HtmlSaveOptions.IsMobileCompatible"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Gibt an, ob das ausgegebene HTML mit mobilen Geräten kompatibel ist. Der Standardwert ist false."
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/ismobilecompatible/
---
## HtmlSaveOptions.IsMobileCompatible property

Gibt an, ob das ausgegebene HTML mit mobilen Geräten kompatibel ist. Der Standardwert ist false.

```csharp
public bool IsMobileCompatible { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsMobileCompatibleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Mobile Compatibility Test");

            // HTML‑Speicheroptionen erstellen
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Mobile Kompatibilität festlegen
            saveOptions.IsMobileCompatible = true;

            // Speichern mit aktivierter mobiler Kompatibilität
            workbook.Save("MobileCompatible.html", saveOptions);

            // Auf nicht-mobil kompatibel ändern
            saveOptions.IsMobileCompatible = false;
            workbook.Save("NonMobileCompatible.html", saveOptions);
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


