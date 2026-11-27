---
title: "StyleFlag.DiagonalUpBorder"
second_title: "Aspose.Cells för .NET API‑referens"
description: "StyleFlag-egenskap. Inställningar för diagonal uppåtriktad kant kommer att tillämpas"
type: docs
url: /sv/net/aspose.cells/styleflag/diagonalupborder/
---
## StyleFlag.DiagonalUpBorder property

Inställningar för diagonal uppåtkant kommer att tillämpas.

```csharp
public bool DiagonalUpBorder { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class StyleFlagPropertyDiagonalUpBorderDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Kom åt cell A1 och ange lite text
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // Skapa ett stilobjekt och sätt diagonal uppåtriktad kant
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.DiagonalUp].LineStyle = CellBorderType.Thick;
            style.Borders[BorderType.DiagonalUp].Color = Color.FromArgb(255, 0, 0, 255);

            // Skapa en stilflagga och aktivera flaggan för diagonal uppåtriktad kant
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.DiagonalUpBorder = true;

            // Tillämpa stilen med flaggan på cellen
            cell.SetStyle(style, styleFlag);

            // Skapa en annan cell för att demonstrera effekten
            Cell cell2 = worksheet.Cells["B2"];
            cell2.PutValue("Diagonal Up Border Demo");

            // Skapa en annan stil för jämförelse
            Style style2 = workbook.CreateStyle();
            style.Borders[BorderType.DiagonalUp].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.DiagonalUp].Color = Color.FromArgb(255, 0, 255, 0);

            // Tillämpa den andra stilen med samma flagga
            cell2.SetStyle(style2, styleFlag);

            // Spara arbetsboken
            workbook.Save("StyleFlagPropertyDiagonalUpBorderDemo.xlsx");
        }
    }
}
```

### Se även

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


