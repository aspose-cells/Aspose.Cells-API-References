---
title: "CellsColor.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CellsColor. Il tipo di colore"
type: docs
url: /it/net/aspose.cells/cellscolor/type/
---
## CellsColor.Type property

Il tipo di colore.

```csharp
public ColorType Type { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una forma per dimostrare CellsColor
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            CellsColor cellsColor = shape.Fill.SolidFill.CellsColor;

            // Mostra il tipo di colore iniziale
            Console.WriteLine("Initial Color Type: " + cellsColor.Type);

            // Imposta il colore RGB e mostra il cambiamento di tipo
            cellsColor.Color = System.Drawing.Color.Red;
            Console.WriteLine("After setting RGB Color - Type: " + cellsColor.Type);

            // Imposta il colore indicizzato e mostra il cambiamento di tipo
            cellsColor.ColorIndex = 5; // Standard Excel color index
            Console.WriteLine("After setting ColorIndex - Type: " + cellsColor.Type);

            // Imposta il colore del tema e mostra il cambiamento di tipo
            cellsColor.ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.0); // Added tint parameter
            Console.WriteLine("After setting ThemeColor - Type: " + cellsColor.Type);

            // Dimostra diversi tipi di colore nelle celle
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

            // Salva il risultato
            workbook.Save("CellsColorTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ColorType](../../colortype/)
* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


