---
title: "HtmlSaveOptions.DisableCss"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions-egenskap. Anger om endast inbäddade stilar ska tillämpas utan att förlita sig på CSS. Standardvärdet är false"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/disablecss/
---
## HtmlSaveOptions.DisableCss property

Anger om endast inline‑stilar ska tillämpas, utan att förlita sig på CSS. Standardvärdet är false.

```csharp
public bool DisableCss { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlSaveOptionsPropertyDisableCssDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata och formatering
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A1"].GetStyle().Font.IsBold = true;
            worksheet.Cells["A1"].GetStyle().Font.Color = System.Drawing.Color.Red;
            worksheet.Cells["B1"].PutValue("Formatted Cell");
            worksheet.Cells["B1"].GetStyle().Font.IsItalic = true;
            worksheet.Cells["B1"].GetStyle().Font.Underline = FontUnderlineType.Single;

            // Skapa en HtmlSaveOptions-instans
            HtmlSaveOptions options = new HtmlSaveOptions();

            // Visa aktuellt DisableCss‑värde
            Console.WriteLine("Current DisableCss value: " + options.DisableCss);

            // Sätt DisableCss till true (använder inbäddade stilar istället för CSS)
            options.DisableCss = true;
            workbook.Save("HtmlWithInlineStyles.html", options);

            // Ställ in DisableCss till false (med CSS-stilar)
            options.DisableCss = false;
            workbook.Save("HtmlWithCssStyles.html", options);

            // Jämför utdatafilerna för att se skillnaden i stilmetod
            Console.WriteLine("Files saved with different DisableCss settings.");
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


