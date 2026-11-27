---
title: "StyleFlag.DiagonalDownBorder"
second_title: "Aspose.Cells för .NET API‑referens"
description: "StyleFlag egenskap. Inställningar för diagonal nedåtriktad kant kommer att tillämpas"
type: docs
url: /sv/net/aspose.cells/styleflag/diagonaldownborder/
---
## StyleFlag.DiagonalDownBorder property

Inställningar för diagonal nedåtkant kommer att tillämpas.

```csharp
public bool DiagonalDownBorder { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class StyleFlagPropertyDiagonalDownBorderDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Kom åt cell A1 och ange lite text
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Diagonal Down Border Demo");

            // Skapa ett stilobjekt och sätt diagonal nedre kant
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.DiagonalDown].LineStyle = CellBorderType.Thick;
            style.Borders[BorderType.DiagonalDown].Color = Color.FromArgb(255, 0, 0, 255);
            
            // Skapa en stilflagga och aktivera diagonal nedre kant-flagga
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.DiagonalDownBorder = true;

            // Tillämpa stilen med flaggan på cellen
            cell.SetStyle(style, styleFlag);

            // Kontrollera om flaggan för diagonal nedre kant är aktiverad
            Console.WriteLine("DiagonalDownBorder flag is enabled: " + cell.GetStyle().Borders[BorderType.DiagonalDown].LineStyle);

            // Inaktivera flaggan för diagonal nedre kant
            styleFlag.DiagonalDownBorder = false;
            style.Borders[BorderType.DiagonalDown].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.DiagonalDown].Color = Color.FromArgb(255, 0, 255, 0);

            // Tillämpa stilen med flaggan på cellen
            cell.SetStyle(style, styleFlag);
            Console.WriteLine("DiagonalDownBorder flag is now: " + cell.GetStyle().Borders[BorderType.DiagonalDown].LineStyle);

            // Spara arbetsboken
            workbook.Save("StyleFlagPropertyDiagonalDownBorderDemo.xlsx");
        }
    }
}
```

### Se även

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


