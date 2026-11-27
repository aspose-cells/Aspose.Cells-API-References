---
title: "CellsColor.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellsColor property. Färgtypen"
type: docs
url: /sv/net/aspose.cells/cellscolor/type/
---
## CellsColor.Type property

Färgtypen.

```csharp
public ColorType Type { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class CellsColorPropertyTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en form för att demonstrera CellsColor
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            CellsColor cellsColor = shape.Fill.SolidFill.CellsColor;

            // Visa initial färgtyp
            Console.WriteLine("Initial Color Type: " + cellsColor.Type);

            // Ställ in RGB-färg och visa typändring
            cellsColor.Color = System.Drawing.Color.Red;
            Console.WriteLine("After setting RGB Color - Type: " + cellsColor.Type);

            // Ställ in indexerad färg och visa typändring
            cellsColor.ColorIndex = 5; // Standard Excel color index
            Console.WriteLine("After setting ColorIndex - Type: " + cellsColor.Type);

            // Ställ in temafärg och visa typändring
            cellsColor.ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.0); // Added tint parameter
            Console.WriteLine("After setting ThemeColor - Type: " + cellsColor.Type);

            // Demonstrera olika färgtyper i celler
            Cell cell1 = worksheet.Cells["A1"];
            cell1.PutValue("RGB Color");
            Style style1 = cell1.GetStyle(); // Use GetStyle() instead of Style property
            style1.ForegroundColor = System.Drawing.Color.Blue;
            style1.Pattern = BackgroundType.Solid;
            cell1.SetStyle(style1);

            Cell cell2 = worksheet.Cells["A2"];
            cell2.PutValue("Indexed Color");
            Style style2 = cell2.GetStyle(); // Use GetStyle() instead of Style property
            style2.ForegroundColor = System.Drawing.Color.FromArgb(5); // Using color index
            style2.Pattern = BackgroundType.Solid;
            cell2.SetStyle(style2);

            // Spara resultatet
            workbook.Save("CellsColorTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ColorType](../../colortype/)
* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


