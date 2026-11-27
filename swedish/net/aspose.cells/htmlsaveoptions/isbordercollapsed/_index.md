---
title: "HtmlSaveOptions.IsBorderCollapsed"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions-egenskap. Anger om tabellramarna är kollapsade. Standardvärdet är true"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/isbordercollapsed/
---
## HtmlSaveOptions.IsBorderCollapsed property

Anger om tabellramarna är sammanslagna. Standardvärdet är true.

```csharp
public bool IsBorderCollapsed { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using System.Threading;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsBorderCollapsedDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata och ramar
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;

            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["B2"].PutValue("With Borders");
            worksheet.Cells["B2"].SetStyle(style);

            // Ställ in kultur för demonstration
            var culture = new System.Globalization.CultureInfo("de-DE");
            Thread.CurrentThread.CurrentCulture = culture;
            Thread.CurrentThread.CurrentUICulture = culture;
            workbook.Settings.CultureInfo = culture;

            // Skapa HTML-sparalternativ och ställ in IsBorderCollapsed
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            saveOptions.IsBorderCollapsed = false;

            // Spara arbetsboken med HTML-alternativ
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "HtmlWithBorders.html");
            workbook.Save(outputPath, saveOptions);

            Console.WriteLine("File saved with collapsed borders: " + outputPath);
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


