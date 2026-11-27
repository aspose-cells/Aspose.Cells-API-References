---
title: "DefaultStyleSettings.FontSize"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Egenskapen DefaultStyleSettings. Hämtar/Anger standardteckensnittets storlek för arbetsboken"
type: docs
url: /sv/net/aspose.cells/defaultstylesettings/fontsize/
---
## DefaultStyleSettings.FontSize property

Hämtar/Anger standardstorleken för standardtypsnittet i arbetsboken.

```csharp
public double FontSize { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DefaultStyleSettingsPropertyFontSizeDemo
    {
        public static void Run()
        {
            HtmlLoadOptions htmlLoadOptions = new HtmlLoadOptions();
            
            // Ange standardteckensnittets namn och storlek
            htmlLoadOptions.DefaultStyleSettings.FontName = "Calibri";
            htmlLoadOptions.DefaultStyleSettings.FontSize = 11.0;

            // Läs in HTML-fil med dessa inställningar
            Workbook workbook = new Workbook("example.html", htmlLoadOptions);

            // Få åtkomst till en cell och visa dess teckensnittsstorlek
            Cell cell = workbook.Worksheets[0].Cells["A1"];
            Console.WriteLine("Cell A1 Font Size: " + cell.GetStyle().Font.Size);
        }
    }
}
```

### Se även

* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


