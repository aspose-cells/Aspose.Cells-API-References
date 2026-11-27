---
title: "HtmlSaveOptions.ExportActiveWorksheetOnly"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions-egenskap. Anger om endast det aktiva kalkylbladet ska exporteras till en html-fil. Om true exporteras endast det aktiva kalkylbladet till html-filen. Om false exporteras hela arbetsboken till html-filen. Standardvärdet är false"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/exportactiveworksheetonly/
---
## HtmlSaveOptions.ExportActiveWorksheetOnly property

Anger om endast det aktiva kalkylbladet ska exporteras till html‑fil. Om true exporteras endast det aktiva kalkylbladet till html‑fil; om false exporteras hela arbetsboken till html‑fil. Standardvärdet är false

```csharp
public bool ExportActiveWorksheetOnly { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportActiveWorksheetOnlyDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med två kalkylblad
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Lägg till exempeldata i båda bladen
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[1].Cells["A1"].PutValue("Sheet2 Data");

            // Ställ in HTML-sparalternativ för att exportera endast det aktiva kalkylbladet
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportActiveWorksheetOnly = true;
            
            // Ställ in det första kalkylbladet som aktivt
            workbook.Worksheets.ActiveSheetIndex = 0;
            
            // Spara med endast det aktiva kalkylbladet
            workbook.Save("output_active_sheet_only.html", saveOptions);
            
            // Byt aktivt blad och spara igen
            workbook.Worksheets.ActiveSheetIndex = 1;
            workbook.Save("output_active_sheet_only2.html", saveOptions);
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


