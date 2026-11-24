---
title: "CellsColor.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellsColor‑Eigenschaft. Der Farbtyp."
type: docs
url: /de/net/aspose.cells/cellscolor/type/
---
## CellsColor.Type property

Der Farbtyp.

```csharp
public ColorType Type { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine Form, um CellsColor zu demonstrieren.
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            CellsColor cellsColor = shape.Fill.SolidFill.CellsColor;

            // Zeige den anfänglichen Farbtyp an.
            Console.WriteLine("Initial Color Type: " + cellsColor.Type);

            // Setze RGB‑Farbe und zeige den Typwechsel.
            cellsColor.Color = System.Drawing.Color.Red;
            Console.WriteLine("After setting RGB Color - Type: " + cellsColor.Type);

            // Setze indizierte Farbe und zeige den Typwechsel.
            cellsColor.ColorIndex = 5; // Standard Excel color index
            Console.WriteLine("After setting ColorIndex - Type: " + cellsColor.Type);

            // Setze Themenfarbe und zeige den Typwechsel.
            cellsColor.ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.0); // Added tint parameter
            Console.WriteLine("After setting ThemeColor - Type: " + cellsColor.Type);

            // Demonstriere verschiedene Farbtypen in Zellen.
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

            // Ergebnis speichern
            workbook.Save("CellsColorTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ColorType](../../colortype/)
* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


