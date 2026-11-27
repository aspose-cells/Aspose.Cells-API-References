---
title: "Style.HasBorders"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style-egenskap. Kontrollerar om det finns några kanter som har satts för stilen"
type: docs
url: /sv/net/aspose.cells/style/hasborders/
---
## Style.HasBorders property

Kontrollerar om det finns kanter som har satts för stilen.

```csharp
public bool HasBorders { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyHasBordersDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Åtkomst till cell A1 och kontrollera om den har kanter (bör vara falskt som standard)
            Cell cellA1 = cells["A1"];
            Console.WriteLine("Cell A1 has borders: " + cellA1.GetStyle().HasBorders);

            // Skapa en stil med kanter
            Style styleWithBorders = workbook.CreateStyle();
            styleWithBorders.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            styleWithBorders.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;

            // Applicera stilen på cell B1
            Cell cellB1 = cells["B1"];
            cellB1.SetStyle(styleWithBorders);

            // Kontrollera om cell B1 har kanter (bör vara sant nu)
            Console.WriteLine("Cell B1 has borders: " + cellB1.GetStyle().HasBorders);

            // Spara arbetsboken
            workbook.Save("HasBordersDemo.xlsx");
        }
    }
}
```

### Se även

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


