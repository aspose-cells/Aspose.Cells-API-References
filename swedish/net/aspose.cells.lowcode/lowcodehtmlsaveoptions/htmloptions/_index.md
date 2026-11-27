---
title: "LowCodeHtmlSaveOptions.HtmlOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LowCodeHtmlSaveOptions egenskap. De allmänna alternativen för att spara html"
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodehtmlsaveoptions/htmloptions/
---
## LowCodeHtmlSaveOptions.HtmlOptions property

De allmänna alternativen för att spara html.

```csharp
public HtmlSaveOptions HtmlOptions { get; set; }
```

### Anmärkningar

När en [`HtmlSaveOptions`](../../../aspose.cells/htmlsaveoptions/) instans anges, kommer [`SaveFormat`](../saveformat/) att skrivas över (om det tidigare har angetts).

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeHtmlSaveOptionsPropertyHtmlOptionsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.99);
            
            // Skapa low-code HTML-sparalternativ
            LowCodeHtmlSaveOptions saveOptions = new LowCodeHtmlSaveOptions
            {
                SaveFormat = SaveFormat.Html,
                HtmlOptions = new HtmlSaveOptions()
            };

            // Visa aktuell exportinställning för rutnät
            Console.WriteLine("Export gridlines initially: " + saveOptions.HtmlOptions.ExportGridLines);

            // Spara med synliga rutnät
            workbook.Save("HtmlWithGridlines.html", saveOptions.HtmlOptions);

            // Ändra HTML-alternativ för att dölja rutnät
            saveOptions.HtmlOptions = new HtmlSaveOptions { ExportGridLines = false };
            Console.WriteLine("Export gridlines after modification: " + saveOptions.HtmlOptions.ExportGridLines);

            // Spara utan rutnät
            workbook.Save("HtmlWithoutGridlines.html", saveOptions.HtmlOptions);

            Console.WriteLine("Demo executed successfully. Compare output files.");
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../../../aspose.cells/htmlsaveoptions/)
* class [LowCodeHtmlSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


