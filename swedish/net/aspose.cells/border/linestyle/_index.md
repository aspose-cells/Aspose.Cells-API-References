---
title: "Border.LineStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Border‑egenskap. Hämtar eller anger cellkantens typ"
type: docs
url: /sv/net/aspose.cells/border/linestyle/
---
## Border.LineStyle property

Hämtar eller anger cellkantens typ.

```csharp
public CellBorderType LineStyle { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BorderPropertyLineStyleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Få åtkomst till en cell och hämta dess stil
            Cell cell = worksheet.Cells["B2"];
            Style style = cell.GetStyle();

            // Ställ in olika kantlinjestilar
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dashed;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dotted;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Double;

            // Tillämpa stilen på cellen
            cell.SetStyle(style);

            // Spara arbetsboken
            workbook.Save("BorderLineStyleDemo.xlsx");
        }
    }
}
```

### Se även

* enum [CellBorderType](../../cellbordertype/)
* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


