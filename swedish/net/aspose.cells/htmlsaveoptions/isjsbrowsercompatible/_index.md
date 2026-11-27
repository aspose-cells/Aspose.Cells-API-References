---
title: "HtmlSaveOptions.IsJsBrowserCompatible"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions-egenskap. Anger om JavaScript är kompatibelt med webbläsare som inte stöder JavaScript. Standardvärdet är true"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/isjsbrowsercompatible/
---
## HtmlSaveOptions.IsJsBrowserCompatible property

Anger om JavaScript är kompatibel med webbläsare som inte stödjer JavaScript. Standardvärdet är true.

```csharp
public bool IsJsBrowserCompatible { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsJsBrowserCompatibleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test JavaScript Compatibility");

            // Konfigurera HTML‑sparalternativ med IsJsBrowserCompatible satt till true
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                IsJsBrowserCompatible = true,
                ExportFormula = true,
                PresentationPreference = true
            };

            // Spara arbetsboken med JavaScript‑kompatibilitet
            workbook.Save("JsCompatibleOutput.html", saveOptions);

            Console.WriteLine("HTML file with JavaScript compatibility saved successfully.");
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


