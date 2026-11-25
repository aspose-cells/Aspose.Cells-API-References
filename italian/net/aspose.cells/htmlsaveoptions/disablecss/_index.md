---
title: "HtmlSaveOptions.DisableCss"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se vengono applicati solo stili inline senza fare affidamento su CSS. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/disablecss/
---
## HtmlSaveOptions.DisableCss property

Indica se vengono applicati solo gli stili inline, senza fare affidamento su CSS. Il valore predefinito è false.

```csharp
public bool DisableCss { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlSaveOptionsPropertyDisableCssDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio e formattazione
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A1"].GetStyle().Font.IsBold = true;
            worksheet.Cells["A1"].GetStyle().Font.Color = System.Drawing.Color.Red;
            worksheet.Cells["B1"].PutValue("Formatted Cell");
            worksheet.Cells["B1"].GetStyle().Font.IsItalic = true;
            worksheet.Cells["B1"].GetStyle().Font.Underline = FontUnderlineType.Single;

            // Crea un'istanza di HtmlSaveOptions
            HtmlSaveOptions options = new HtmlSaveOptions();

            // Visualizza il valore corrente di DisableCss
            Console.WriteLine("Current DisableCss value: " + options.DisableCss);

            // Imposta DisableCss su true (usando stili inline invece di CSS)
            options.DisableCss = true;
            workbook.Save("HtmlWithInlineStyles.html", options);

            // Imposta DisableCss su false (usando stili CSS)
            options.DisableCss = false;
            workbook.Save("HtmlWithCssStyles.html", options);

            // Confronta i file di output per vedere la differenza nell'approccio di stile
            Console.WriteLine("Files saved with different DisableCss settings.");
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


