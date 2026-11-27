---
title: "Font.Underline"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Font-egenskap. Hämtar eller anger fontens understrykningstyp"
type: docs
url: /sv/net/aspose.cells/font/underline/
---
## Font.Underline property

Hämtar eller anger understrykningsstilen för teckensnittet.

```csharp
public FontUnderlineType Underline { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyUnderlineDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Kom åt cellen och ange understrykningsstil
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Sample Underlined Text");
            
            // Hämta stilen och ändra font-egenskaper
            Style style = cell.GetStyle();
            style.Font.Underline = FontUnderlineType.Single;
            cell.SetStyle(style);

            // Spara arbetsboken
            workbook.Save("FontUnderlineDemo.xlsx");
        }
    }
}
```

### Se även

* enum [FontUnderlineType](../../fontunderlinetype/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


