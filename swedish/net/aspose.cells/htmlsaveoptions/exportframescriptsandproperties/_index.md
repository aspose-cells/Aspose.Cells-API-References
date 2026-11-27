---
title: "HtmlSaveOptions.ExportFrameScriptsAndProperties"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions egenskap. Anger om ram-skript och dokumentegenskaper ska exporteras. Standardvärdet är true. Om du vill importera html- eller mht-filen till Excel, behåll standardvärdet"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/exportframescriptsandproperties/
---
## HtmlSaveOptions.ExportFrameScriptsAndProperties property

Anger om ram-skript och dokumentegenskaper ska exporteras. Standardvärdet är true. Om du vill importera html- eller mht-filen till Excel, behåll standardvärdet.

```csharp
public bool ExportFrameScriptsAndProperties { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportFrameScriptsAndPropertiesDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // Ställ in HTML-sparalternativ med ExportFrameScriptsAndProperties
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportFrameScriptsAndProperties = true;

            // Spara som HTML
            workbook.Save("output.html", options);

            Console.WriteLine("HTML file saved with ExportFrameScriptsAndProperties enabled.");
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


