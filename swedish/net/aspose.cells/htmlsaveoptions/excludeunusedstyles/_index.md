---
title: "HtmlSaveOptions.ExcludeUnusedStyles"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions-egenskap. Anger om oanvända stilar exkluderas. För de genererade HTML-filerna kan uteslutning av oanvända stilar göra filstorleken mindre utan att påverka de visuella effekterna. Så standardvärdet för denna egenskap är true. Om användaren behöver behålla alla stilar i arbetsboken för den genererade HTML:n, till exempel i scenariot där användaren senare måste återställa arbetsboken från den genererade HTML:n, sätt denna egenskap till false."
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/excludeunusedstyles/
---
## HtmlSaveOptions.ExcludeUnusedStyles property

Anger om oanvända stilar ska uteslutas. För de genererade html‑filerna kan uteslutning av oanvända stilar göra filstorleken mindre utan att påverka den visuella effekten. Så standardvärdet för denna egenskap är true. Om användaren behöver behålla alla stilar i arbetsboken för den genererade html‑filen (t.ex. i scenariot där arbetsboken ska återställas från den genererade html‑filen senare), sätt denna egenskap till false.

```csharp
public bool ExcludeUnusedStyles { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExcludeUnusedStylesDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till exempeldata med olika stilar
            Cell cell1 = workbook.Worksheets[0].Cells["A1"];
            cell1.Value = "Styled text";
            Style style1 = cell1.GetStyle();
            style1.Font.Color = Color.Red;
            style1.Font.IsBold = true;
            cell1.SetStyle(style1);

            Cell cell2 = workbook.Worksheets[0].Cells["A2"];
            cell2.Value = "Different style";
            Style style2 = cell2.GetStyle();
            style2.Font.Name = "Times New Roman";
            style2.Font.Size = 14;
            cell2.SetStyle(style2);

            // Konfigurera HTML-sparalternativ för att exkludera oanvända stilar
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExcludeUnusedStyles = true;

            // Spara arbetsboken med HTML-alternativ
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);

            Console.WriteLine("HTML file saved with ExcludeUnusedStyles=true");
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


