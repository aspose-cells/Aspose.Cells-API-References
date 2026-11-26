---
title: "Range.SetInsideBorders"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Range. Establece los bordes internos del rango"
type: docs
url: /es/net/aspose.cells/range/setinsideborders/
---
## Range.SetInsideBorders method

Establece los bordes internos del rango.

```csharp
public void SetInsideBorders(BorderType borderEdge, CellBorderType lineStyle, 
    CellsColor borderColor)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| borderEdge | BorderType | Tipo de borde interno, solo puede ser Vertical y Horizontal. |
| lineStyle | CellBorderType | El estilo del borde. |
| borderColor | CellsColor | El color del borde. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RangeMethodSetInsideBordersWithBorderTypeCellBorderTypeCellsCDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un rango y establece bordes internos
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B5:F10");
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            range.SetInsideBorders(BorderType.Vertical, CellBorderType.Thin, color);

            // Verifica los bordes en una celda dentro del rango
            Cell cell = worksheet.Cells["C6"];
            Style style = cell.GetStyle();
            Console.WriteLine("Left Border: " + style.Borders[BorderType.LeftBorder].LineStyle);
            Console.WriteLine("Right Border: " + style.Borders[BorderType.RightBorder].LineStyle);
            Console.WriteLine("Top Border: " + style.Borders[BorderType.TopBorder].LineStyle);
            Console.WriteLine("Bottom Border: " + style.Borders[BorderType.BottomBorder].LineStyle);

            workbook.Save("SetInsideBordersExample.xlsx");
        }
    }
}
```

### Ver también

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [CellsColor](../../cellscolor/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


