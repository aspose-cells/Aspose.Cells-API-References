---
title: "HtmlSaveOptions.ExportHiddenWorksheet"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions-egenskap. Anger om det dolda kalkylbladets innehåll ska exporteras. Standardvärdet är true"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/exporthiddenworksheet/
---
## HtmlSaveOptions.ExportHiddenWorksheet property

Anger om dolt kalkylbladsinnehåll ska exporteras. Standardvärdet är true.

```csharp
public bool ExportHiddenWorksheet { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportHiddenWorksheetDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet1 = workbook.Worksheets[0];
            worksheet1.Name = "VisibleSheet";
            worksheet1.Cells["A1"].PutValue("Visible Data");

            Worksheet worksheet2 = workbook.Worksheets.Add("HiddenSheet");
            worksheet2.Cells["A1"].PutValue("Hidden Data");
            worksheet2.IsVisible = false;

            // Ställ in HTML‑sparalternativ
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                ExportHiddenWorksheet = false, // Don't export hidden worksheets
                ExportActiveWorksheetOnly = false
            };

            // Spara utan att exportera dolda kalkylblad
            workbook.Save("output_without_hidden.html", saveOptions);

            // Ändra alternativet för att exportera dolda kalkylblad
            saveOptions.ExportHiddenWorksheet = true;

            // Spara med dolda kalkylblad exporterade
            workbook.Save("output_with_hidden.html", saveOptions);
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


