---
title: "Style.BackgroundColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style-egenskap. Hämtar eller anger en stils bakgrundsfärg"
type: docs
url: /sv/net/aspose.cells/style/backgroundcolor/
---
## Style.BackgroundColor property

Hämtar eller anger en stils bakgrundsfärg.

```csharp
public Color BackgroundColor { get; set; }
```

### Anmärkningar

Om du vill ange en cells färg, använd Style.ForegroundColor-egenskapen. Endast om cellstilens mönster är annat än ingen eller solid, kommer denna egenskap att ha effekt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyBackgroundColorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa ett stilobjekt
            Style style = workbook.CreateStyle();
            
            // Ange bakgrundsfärg till gul
            style.BackgroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            
            // Applicera stilen på cell A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Cell with yellow background");
            cell.SetStyle(style);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


