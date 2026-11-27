---
title: "Border.Color"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Border‑egenskap. Hämtar eller anger färgen på kanten"
type: docs
url: /sv/net/aspose.cells/border/color/
---
## Border.Color property

Hämtar eller anger färgen på kanten.

```csharp
public Color Color { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class BorderPropertyColorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Åtkomst till cell A1
            Cell cell = worksheet.Cells["A1"];
            
            // Ange cellvärdet
            cell.PutValue("Border Color Demo");
            
            // Hämta cellens stil
            Style style = cell.GetStyle();
            
            // Ställ in kantfärger och stilar
            style.Borders[BorderType.TopBorder].Color = Color.Red;
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            
            style.Borders[BorderType.BottomBorder].Color = Color.Blue;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dotted;
            
            style.Borders[BorderType.LeftBorder].Color = Color.Green;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dashed;
            
            style.Borders[BorderType.RightBorder].Color = Color.FromArgb(255, 128, 0); // Orange
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            
            // Tillämpa stilen på cellen
            cell.SetStyle(style);
            
            // Spara arbetsboken
            workbook.Save("BorderColorDemo.xlsx");
            
            Console.WriteLine("Border color demo created successfully.");
        }
    }
}
```

### Se även

* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


