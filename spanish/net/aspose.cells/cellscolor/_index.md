---
title: "Clase CellsColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.CellsColor. Representa todos los tipos de color"
type: docs
url: /es/net/aspose.cells/cellscolor/
---
## CellsColor class

Representa todos los tipos de color.

```csharp
public class CellsColor
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Argb](../../aspose.cells/cellscolor/argb/) { get; set; } | Obtiene y establece el color a partir de un valor ARGB de 32 bits. |
| [Color](../../aspose.cells/cellscolor/color/) { get; set; } | Obtiene y establece el color RGB. |
| [ColorIndex](../../aspose.cells/cellscolor/colorindex/) { get; set; } | Obtiene y establece el índice de color en la paleta de colores. Solo se aplica a colores indexados. |
| [IsShapeColor](../../aspose.cells/cellscolor/isshapecolor/) { get; set; } | Obtiene y establece el color que debe aplicarse a la celda o forma. |
| [ThemeColor](../../aspose.cells/cellscolor/themecolor/) { get; set; } | Obtiene el color del tema. Solo se aplica al tipo de color de tema. |
| [Transparency](../../aspose.cells/cellscolor/transparency/) { get; set; } | Obtiene y establece la transparencia como un valor de 0.0 (opaco) a 1.0 (transparente). |
| [Type](../../aspose.cells/cellscolor/type/) { get; } | El tipo de color. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [SetTintOfShapeColor](../../aspose.cells/cellscolor/settintofshapecolor/)(double) | Establecer el tono del color de la forma |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellsColorDemo
    {
        public static void CellsColorExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un rango de celdas
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "A10");

            // Crear una instancia de CellsColor
            CellsColor cellsColor = workbook.CreateCellsColor();

            // Establecer propiedades de CellsColor
            cellsColor.IsShapeColor = false;
            cellsColor.Color = Color.Red;
            cellsColor.ColorIndex = 5;
            cellsColor.Argb = Color.Blue.ToArgb();
            cellsColor.Transparency = 0.5;

            // Aplicar CellsColor al rango
            Style style = workbook.CreateStyle();
            style.ForegroundColor = cellsColor.Color;
            style.Pattern = BackgroundType.Solid;
            range.ApplyStyle(style, new StyleFlag { CellShading = true });

            // Guarda el libro de trabajo
            workbook.Save("CellsColorExample.xlsx");
            workbook.Save("CellsColorExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


