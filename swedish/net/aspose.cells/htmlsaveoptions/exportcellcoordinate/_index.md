---
title: "HtmlSaveOptions.ExportCellCoordinate"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions-egenskap. Anger om koordinater för icke‑tomma celler i Excel exporteras när filen sparas till HTML. Standardvärdet är false. Om du vill importera den genererade HTML:n till Excel, behåll standardvärdet."
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/exportcellcoordinate/
---
## HtmlSaveOptions.ExportCellCoordinate property

Anger om Excel-koordinater för icke-tomma celler ska exporteras när filen sparas som html. Standardvärdet är false. Om du vill importera den exporterade html-filen till Excel, behåll standardvärdet.

```csharp
public bool ExportCellCoordinate { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportCellCoordinateDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            // Skapa HTML-sparalternativ och aktivera ExportCellCoordinate
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportCellCoordinate = true;

            // Spara arbetsboken som HTML med cellkoordinater
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML with cell coordinates exported successfully.");
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


