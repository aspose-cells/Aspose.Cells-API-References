---
title: "Row.GetStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Row metod. Hämtar stilen för denna rad"
type: docs
url: /sv/net/aspose.cells/row/getstyle/
---
## Row.GetStyle method

Hämtar stilen för den här raden.

```csharp
public Style GetStyle()
```

### Anmärkningar

Att ändra det returnerade stilobjektet direkt har ingen effekt för den här raden eller någon cell i raden. Du måste anropa [`ApplyStyle`](../applystyle/) eller [`SetStyle`](../setstyle/) metod för att tillämpa ändringen på den här raden. Radvärldens stil är den stil som ärvs av cellerna i raden (de celler som inte har anpassade stilinställningar, såsom befintliga celler som inte har fått stil explicit, eller de som inte har instansierats)

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowMethodGetStyleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ställ in stilar för demonstration
            Style rowStyle = workbook.CreateStyle();
            rowStyle.Pattern = BackgroundType.Solid;
            rowStyle.ForegroundColor = System.Drawing.Color.Blue;
            cells.Rows[8].ApplyStyle(rowStyle, new StyleFlag { All = true });

            Style columnStyle = workbook.CreateStyle();
            columnStyle.Pattern = BackgroundType.Solid;
            columnStyle.ForegroundColor = System.Drawing.Color.Red;
            cells.Columns[5].ApplyStyle(columnStyle, new StyleFlag { All = true });

            // Demonstrera användning av GetStyle
            Style retrievedRowStyle = cells.Rows[8].GetStyle();
            Console.WriteLine("Row 8 Style - ForegroundColor: " + retrievedRowStyle.ForegroundColor);
            Console.WriteLine("Row 8 Style - Pattern: " + retrievedRowStyle.Pattern);

            Style retrievedColumnStyle = cells.Columns[5].GetStyle();
            Console.WriteLine("Column 5 Style - ForegroundColor: " + retrievedColumnStyle.ForegroundColor);
            Console.WriteLine("Column 5 Style - Pattern: " + retrievedColumnStyle.Pattern);
        }
    }
}
```

### Se även

* class [Style](../../style/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


