---
title: "HtmlSaveOptions.ExportWorksheetProperties"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions-egenskap. Anger om arbetsblads egenskaper exporteras. Standardvärdet är true. Om du vill importera html- eller mht-filen till Excel, behåll standardvärdet."
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/exportworksheetproperties/
---
## HtmlSaveOptions.ExportWorksheetProperties property

Anger om kalkylblads egenskaper ska exporteras. Standardvärdet är true. Om du vill importera html- eller mht-filen till Excel, behåll standardvärdet.

```csharp
public bool ExportWorksheetProperties { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportWorksheetPropertiesDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok med testdata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Data");

            // Ställ in HTML‑sparalternativ med ExportWorksheetProperties inaktiverat
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportWorksheetProperties = false;
            
            // Spara med arbetsblads‑egenskaper inaktiverade
            workbook.Save("output_without_worksheet_props.html", options);

            // Aktivera export av arbetsblads‑egenskaper
            options.ExportWorksheetProperties = true;
            
            // Spara med arbetsblads‑egenskaper aktiverade
            workbook.Save("output_with_worksheet_props.html", options);
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


