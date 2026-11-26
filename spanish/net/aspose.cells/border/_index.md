---
title: "Clase Border"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Border. Encapsula el objeto que representa el borde de la celda"
type: docs
url: /es/net/aspose.cells/border/
---
## Border class

Encapsula el objeto que representa el borde de la celda.

```csharp
public class Border
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ArgbColor](../../aspose.cells/border/argbcolor/) { get; set; } | Obtiene y establece el color con un valor ARGB de 32 bits. |
| [Color](../../aspose.cells/border/color/) { get; set; } | Obtiene o establece el color del borde. |
| [LineStyle](../../aspose.cells/border/linestyle/) { get; set; } | Obtiene o establece el tipo de borde de la celda. |
| [ThemeColor](../../aspose.cells/border/themecolor/) { get; set; } | Obtiene y establece el color temático del borde. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class BorderDemo
    {
        public static void BorderExample()
        {
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();

            // Añadiendo una nueva hoja de cálculo al objeto Workbook
            workbook.Worksheets.Add();

            // Obteniendo la referencia de la hoja de cálculo recién añadida pasando su índice de hoja
            Worksheet worksheet = workbook.Worksheets[0];

            // Accediendo a la celda "A1" de la hoja de cálculo
            Cell cell = worksheet.Cells["A1"];

            // Añadiendo un valor a la celda "A1"
            cell.PutValue("Hello World");

            // Obteniendo el estilo de la celda
            Style style = cell.GetStyle();

            // Estableciendo el estilo de línea del borde superior
            Border topBorder = style.Borders[BorderType.TopBorder];
            topBorder.LineStyle = CellBorderType.Medium;
            topBorder.Color = Color.Red;

            // Estableciendo el estilo de línea del borde inferior
            Border bottomBorder = style.Borders[BorderType.BottomBorder];
            bottomBorder.LineStyle = CellBorderType.Thick;
            bottomBorder.Color = Color.Blue;

            // Estableciendo el estilo de línea del borde izquierdo
            Border leftBorder = style.Borders[BorderType.LeftBorder];
            leftBorder.LineStyle = CellBorderType.Dashed;
            leftBorder.Color = Color.Green;

            // Estableciendo el estilo de línea del borde derecho
            Border rightBorder = style.Borders[BorderType.RightBorder];
            rightBorder.LineStyle = CellBorderType.Dotted;
            rightBorder.Color = Color.Purple;

            // Aplicando el estilo a la celda
            cell.SetStyle(style);

            // Guardando el archivo Excel
            workbook.Save("BorderExample.xlsx");
            workbook.Save("BorderExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


