---
title: "CellsColor.Color"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CellsColor. Obtiene y establece el color RGB"
type: docs
url: /es/net/aspose.cells/cellscolor/color/
---
## CellsColor.Color property

Obtiene y establece el color RGB.

```csharp
public Color Color { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellsColorPropertyColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un rango y establecer bordes coloreados
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B5:F10");
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            range.SetInsideBorders(BorderType.Horizontal | BorderType.Vertical, CellBorderType.Thin, color);

            // Verificar la configuración de bordes en una celda
            Cell cell = worksheet.Cells["F5"];
            Style style = cell.GetStyle();
            Console.WriteLine("Left Border: " + style.Borders[BorderType.LeftBorder].LineStyle);
            Console.WriteLine("Bottom Border: " + style.Borders[BorderType.BottomBorder].LineStyle);

            // Guarda el libro de trabajo
            workbook.Save("CellsColorPropertyColorDemo.xlsx");
        }
    }
}
```

### Ver también

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


