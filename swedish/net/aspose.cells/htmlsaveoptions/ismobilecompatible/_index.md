---
title: "HtmlSaveOptions.IsMobileCompatible"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions‑egenskap. Anger om den genererade HTML‑koden är kompatibel med mobila enheter. Standardvärdet är falskt"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/ismobilecompatible/
---
## HtmlSaveOptions.IsMobileCompatible property

Anger om den genererade HTML-koden är kompatibel med mobila enheter. Standardvärdet är false.

```csharp
public bool IsMobileCompatible { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsMobileCompatibleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Mobile Compatibility Test");

            // Skapa HTML-sparalternativ
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Ställ in mobil kompatibilitet
            saveOptions.IsMobileCompatible = true;

            // Spara med mobil kompatibilitet aktiverad
            workbook.Save("MobileCompatible.html", saveOptions);

            // Ändra till icke-mobil kompatibel
            saveOptions.IsMobileCompatible = false;
            workbook.Save("NonMobileCompatible.html", saveOptions);
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


