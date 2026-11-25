---
title: "CellsColor.ThemeColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CellsColor. Ottiene il colore del tema. Si applica solo al tipo di colore del tema"
type: docs
url: /it/net/aspose.cells/cellscolor/themecolor/
---
## CellsColor.ThemeColor property

Ottiene il colore del tema. Si applica solo al tipo di colore del tema.

```csharp
public ThemeColor ThemeColor { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellsColorPropertyThemeColorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Crea un'istanza di CellsColor
                CellsColor cellsColor = workbook.CreateCellsColor();

                // Imposta un colore del tema
                cellsColor.ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);

                // Visualizza le proprietà di ThemeColor
                Console.WriteLine("ThemeColor Type: " + cellsColor.ThemeColor.ColorType);
                Console.WriteLine("ThemeColor Tint: " + cellsColor.ThemeColor.Tint);

                // Applica il colore a una cella
                Style style = workbook.CreateStyle();
                style.ForegroundColor = cellsColor.Color;
                style.Pattern = BackgroundType.Solid;

                worksheet.Cells["A1"].PutValue("Theme Color Example");
                worksheet.Cells["A1"].SetStyle(style);

                // Salva la cartella di lavoro
                workbook.Save("ThemeColorDemo.xlsx");
                Console.WriteLine("ThemeColor has been demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [ThemeColor](../../themecolor/)
* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


