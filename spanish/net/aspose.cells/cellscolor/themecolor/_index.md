---
title: "CellsColor.ThemeColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CellsColor. Obtiene el color del tema. Solo se aplica al tipo de color de tema"
type: docs
url: /es/net/aspose.cells/cellscolor/themecolor/
---
## CellsColor.ThemeColor property

Obtiene el color del tema. Solo se aplica al tipo de color de tema.

```csharp
public ThemeColor ThemeColor { get; set; }
```

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Crear una instancia de CellsColor
                CellsColor cellsColor = workbook.CreateCellsColor();

                // Establecer un color de tema
                cellsColor.ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);

                // Mostrar las propiedades ThemeColor
                Console.WriteLine("ThemeColor Type: " + cellsColor.ThemeColor.ColorType);
                Console.WriteLine("ThemeColor Tint: " + cellsColor.ThemeColor.Tint);

                // Aplicar el color a una celda
                Style style = workbook.CreateStyle();
                style.ForegroundColor = cellsColor.Color;
                style.Pattern = BackgroundType.Solid;

                worksheet.Cells["A1"].PutValue("Theme Color Example");
                worksheet.Cells["A1"].SetStyle(style);

                // Guarda el libro de trabajo
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

### Ver también

* class [ThemeColor](../../themecolor/)
* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


