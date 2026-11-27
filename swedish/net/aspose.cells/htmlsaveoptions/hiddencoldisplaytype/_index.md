---
title: "HtmlSaveOptions.HiddenColDisplayType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions property. Dold kolumn – bredden på denna kolumn är 0 i Excel innan den sparas i HTML‑format. Om HtmlHiddenColDisplayType är Remove kommer den dolda kolumnen inte att skrivas ut; om värdet är Hidden kommer kolumnen att skrivas ut men vara dold. Standardvärdet är Hidden."
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/hiddencoldisplaytype/
---
## HtmlSaveOptions.HiddenColDisplayType property

Dold kolumn (bredden på den här kolumnen är 0) i Excel, innan du sparar detta i HTML-format, om HtmlHiddenColDisplayType är "Remove" kommer den dolda kolumnen inte att skrivas ut, om värdet är "Hidden" kommer kolumnen att skrivas ut men vara dold, standardvärdet är "Hidden"

```csharp
public HtmlHiddenColDisplayType HiddenColDisplayType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyHiddenColDisplayTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Dölj kolumn C (index 2)
            worksheet.Cells.HideColumn(2);

            // Lägg till lite data för att demonstrera
            worksheet.Cells["A1"].PutValue("Visible Column A");
            worksheet.Cells["B1"].PutValue("Visible Column B");
            worksheet.Cells["C1"].PutValue("Hidden Column C");
            worksheet.Cells["D1"].PutValue("Visible Column D");

            // Skapa HTML‑sparalternativ med olika inställningar för HiddenColDisplayType
            HtmlSaveOptions optionsRemove = new HtmlSaveOptions
            {
                HiddenColDisplayType = HtmlHiddenColDisplayType.Remove
            };

            HtmlSaveOptions optionsHidden = new HtmlSaveOptions
            {
                HiddenColDisplayType = HtmlHiddenColDisplayType.Hidden
            };

            // Spara med olika alternativ
            workbook.Save("output_remove.html", optionsRemove); // Column C will be removed
            workbook.Save("output_hidden.html", optionsHidden); // Column C will be hidden but space preserved
        }
    }
}
```

### Se även

* enum [HtmlHiddenColDisplayType](../../htmlhiddencoldisplaytype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


