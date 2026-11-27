---
title: "HtmlSaveOptions.ShowAllSheets"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions-egenskap. Anger om alla blad ska visas när man sparar som en enda html-fil"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/showallsheets/
---
## HtmlSaveOptions.ShowAllSheets property

Anger om alla blad ska visas när man sparar som en enda HTML-fil.

```csharp
public bool ShowAllSheets { get; set; }
```

### Anmärkningar

Fungerar endast när [`SaveAsSingleFile`](../saveassinglefile/) är True.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyShowAllSheetsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med flera blad
            Workbook workbook = new Workbook();
            
            // Lägg till data i det första bladet
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Name = "FirstSheet";
            sheet1.Cells["A1"].PutValue("Sheet 1 Content");

            // Lägg till ett andra blad
            Worksheet sheet2 = workbook.Worksheets.Add("SecondSheet");
            sheet2.Cells["B2"].PutValue("Sheet 2 Content");

            // Lägg till ett tredje blad
            Worksheet sheet3 = workbook.Worksheets.Add("ThirdSheet");
            sheet3.Cells["C3"].PutValue("Sheet 3 Content");

            // Skapa HTML-sparalternativ
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Ställ in ShowAllSheets-egenskapen till true för att exportera alla blad
            saveOptions.ShowAllSheets = true;

            // Spara arbetsboken med alla blad synliga i HTML
            workbook.Save("ShowAllSheetsDemo.html", saveOptions);

            Console.WriteLine("HTML file with all sheets exported successfully.");
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


