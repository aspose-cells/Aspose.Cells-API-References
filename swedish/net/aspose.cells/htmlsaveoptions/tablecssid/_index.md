---
title: "HtmlSaveOptions.TableCssId"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions‑egenskap. Hämtar och anger prefixet för typ‑css‑namnet, såsom trcoltd osv., som finns i tabell‑elementet som har det specifika TableCssId‑attributet. Standardvärdet är"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/tablecssid/
---
## HtmlSaveOptions.TableCssId property

Hämtar och anger prefixet för typ‑css‑namnet såsom tr, col, td osv, de finns i tabell‑elementet som har det specifika TableCssId‑attributet. Standardvärdet är "".

```csharp
public string TableCssId { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyTableCssIdDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok med testdata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Konfigurera HTML‑sparalternativ med TableCssId
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            saveOptions.TableCssId = "custom-table-style";
            
            // Spara arbetsboken med HTML-alternativ
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML file saved with TableCssId: " + saveOptions.TableCssId);
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


