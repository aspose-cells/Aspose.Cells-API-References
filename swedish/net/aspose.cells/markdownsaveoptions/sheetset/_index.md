---
title: "MarkdownSaveOptions.SheetSet"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MarkdownSaveOptions‑egenskap. Hämtar eller anger vilka blad som ska renderas. Standard är alla synliga blad i den aktiva arbetsboken"
type: docs
url: /sv/net/aspose.cells/markdownsaveoptions/sheetset/
---
## MarkdownSaveOptions.SheetSet property

Hämtar eller anger bladen som ska renderas. Standard är alla synliga blad i arbetsboken: [`Active`](../../../aspose.cells.rendering/sheetset/active/).

```csharp
public SheetSet SheetSet { get; set; }
```

### Anmärkningar

Inställningen ignoreras när den används i [`SheetRender`](../../../aspose.cells.rendering/sheetrender/)

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markdown;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class MarkdownSaveOptionsPropertySheetSetDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Cells["A1"].PutValue("Sheet1 Data");
            
            // Lägg till ett andra kalkylblad
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            sheet2.Cells["A1"].PutValue("Sheet2 Data");

            // Skapa Markdown‑sparalternativ
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
            saveOptions.TableHeaderType = MarkdownTableHeaderType.FirstRow;
            
            // Spara alla blad till markdown
            saveOptions.SheetSet = SheetSet.All;
            workbook.Save("output_all_sheets.md", saveOptions);
            
            // Spara endast det första bladet
            saveOptions.SheetSet = new SheetSet(new int[] { 0 });
            workbook.Save("output_first_sheet.md", saveOptions);
        }
    }
}
```

### Se även

* class [SheetSet](../../../aspose.cells.rendering/sheetset/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


