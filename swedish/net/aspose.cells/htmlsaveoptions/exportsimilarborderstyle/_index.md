---
title: "HtmlSaveOptions.ExportSimilarBorderStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions egenskap. Anger om liknande kantstil ska exporteras när kantstilen inte stöds av webbläsare. Om du vill importera html‑ eller mht‑filen till Excel, behåll standardvärdet. Standardvärdet är falskt."
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/exportsimilarborderstyle/
---
## HtmlSaveOptions.ExportSimilarBorderStyle property

Anger om liknande ramstil ska exporteras när ramstilen inte stöds av webbläsare. Om du vill importera html- eller mht-filen till Excel, behåll standardvärdet. Standardvärdet är false.

```csharp
public bool ExportSimilarBorderStyle { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportSimilarBorderStyleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata med kanter
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A1"].SetStyle(CreateBorderStyle(workbook, CellBorderType.Medium));
            worksheet.Cells["B1"].PutValue("Similar Border");
            worksheet.Cells["B1"].SetStyle(CreateBorderStyle(workbook, CellBorderType.Medium));
            worksheet.Cells["C1"].PutValue("Different Border");
            worksheet.Cells["C1"].SetStyle(CreateBorderStyle(workbook, CellBorderType.Thin));

            // Skapa HTML-sparalternativ
            HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions(SaveFormat.Html)
            {
                ExportSimilarBorderStyle = true // Demonstrate the property
            };

            // Spara arbetsboken
            workbook.Save("output.html", htmlSaveOptions);
        }

        private static Style CreateBorderStyle(Workbook workbook, CellBorderType borderType)
        {
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.TopBorder].LineStyle = borderType;
            style.Borders[BorderType.BottomBorder].LineStyle = borderType;
            style.Borders[BorderType.LeftBorder].LineStyle = borderType;
            style.Borders[BorderType.RightBorder].LineStyle = borderType;
            return style;
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


