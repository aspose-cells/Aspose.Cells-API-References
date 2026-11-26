---
title: "Enumeración BorderType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.BorderType enum. Enumera los tipos de línea de borde y línea diagonal"
type: docs
url: /es/net/aspose.cells/bordertype/
---
## BorderType enumeration

Enumera los tipos de líneas de borde y líneas diagonales.

```csharp
[Flags]
public enum BorderType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| LeftBorder | `1` | Representa la línea de borde izquierda. |
| RightBorder | `2` | Representa la línea de borde derecha existente. |
| TopBorder | `4` | Representa la línea de borde superior. |
| BottomBorder | `8` | Representa la línea de borde inferior. |
| DiagonalDown | `10` | Representa la línea diagonal desde la esquina superior izquierda hasta la esquina inferior derecha. |
| DiagonalUp | `20` | Representa la línea diagonal desde la esquina inferior izquierda hasta la esquina superior derecha. |
| Vertical | `40` | Solo para estilo dinámico, como formato condicional, tabla dinámica. |
| Horizontal | `80` | Solo para estilo dinámico, como formato condicional, tabla dinámica. |
| SideBorders | `F` | Indica los cuatro bordes laterales: LeftBorder, RightBorder, TopBorder y BottomBorder. |
| Diagonal | `30` | Combinación especial de múltiples bordes para la comodidad del usuario en algunas API. Indica los bordes diagonales de DiagonalUp y DiagonalDown. |
| DynamicStyleBorders | `C0` | Indica vertical y horizontal del estilo dinámico. |
| None | `0` | No se ha especificado ningún borde. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class BorderTypeDemo
    {
        public static void BorderTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            // Crear un rango de celdas
            var range = worksheet.Cells.CreateRange("A1:D4");

            // Cree un objeto de estilo
            Style style = workbook.CreateStyle();
            // Establecer los bordes para el rango
            style.SetBorder(BorderType.LeftBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.RightBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.TopBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.DiagonalDown, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.DiagonalUp, CellBorderType.Thin, Color.Blue);

            // Aplicar el estilo al rango
            StyleFlag flag = new StyleFlag { Borders = true };
            range.ApplyStyle(style, flag);

            // Guarda el libro de trabajo
            workbook.Save("BorderTypeExample.xlsx");
            workbook.Save("BorderTypeExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


