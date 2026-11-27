---
title: "HtmlSaveOptions.ExportArea"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions-egenskap. Hämtar eller anger det exporterade CellArea för det aktuella aktiva kalkylbladet. Om du anger detta attribut kommer utskriftsområdet för det aktuella aktiva kalkylbladet att utelämnas. Endast det specificerade området exporteras när filen sparas till HTML."
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/exportarea/
---
## HtmlSaveOptions.ExportArea property

Hämtar eller anger det exporterade CellArea för det aktuella aktiva kalkylbladet. Om du anger detta attribut kommer utskriftsområdet för det aktuella aktiva kalkylbladet att utelämnas. Endast det angivna området kommer att exporteras när filen sparas som html.

```csharp
public CellArea ExportArea { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportAreaDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i lite data i kalkylbladet
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Cell {i},{j}");
                }
            }

            // Ställ in HTML-sparalternativ med exportområde
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportArea = CellArea.CreateCellArea("B2", "D5");

            // Spara arbetsboken med angivet exportområde
            workbook.Save("output.html", options);
        }
    }
}
```

### Se även

* struct [CellArea](../../cellarea/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


