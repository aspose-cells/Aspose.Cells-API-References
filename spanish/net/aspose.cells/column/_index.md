---
title: "Clase Column"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Column clase. Representa una sola columna en una hoja de cálculo"
type: docs
url: /es/net/aspose.cells/column/
---
## Column class

Representa una única columna en una hoja de cálculo.

```csharp
public class Column
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [GroupLevel](../../aspose.cells/column/grouplevel/) { get; set; } | Obtiene el nivel de grupo de la columna. |
| [HasCustomStyle](../../aspose.cells/column/hascustomstyle/) { get; } | Indica si esta columna tiene configuraciones de estilo personalizadas (diferentes de la predeterminada heredada del libro). |
| [Index](../../aspose.cells/column/index/) { get; } | Obtiene el índice de esta columna. |
| [IsCollapsed](../../aspose.cells/column/iscollapsed/) { get; set; } | si la columna está colapsada |
| [IsHidden](../../aspose.cells/column/ishidden/) { get; set; } | Indica si la columna está oculta. |
| [Style](../../aspose.cells/column/style/) { get; } | (**Obsoleto.**) Obtiene el estilo de esta columna. |
| [Width](../../aspose.cells/column/width/) { get; set; } | Obtiene y establece el ancho de la columna en unidades de caracteres. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [ApplyStyle](../../aspose.cells/column/applystyle/)(Style, StyleFlag) | Aplica formatos a toda una columna. |
| [GetStyle](../../aspose.cells/column/getstyle/)() | Obtiene el estilo de esta columna. |
| [SetStyle](../../aspose.cells/column/setstyle/)(Style) | Establece el estilo de esta columna. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColumnDemo
    {
        public static void ColumnExample()
        {
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();

            // Obteniendo la referencia de la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar nuevo estilo al libro de trabajo
            Style style = workbook.CreateStyle();

            // Estableciendo el color de fondo a azul
            style.BackgroundColor = Color.Blue;

            // Estableciendo el color de primer plano a rojo
            style.ForegroundColor = Color.Red;

            // Estableciendo el patrón de fondo
            style.Pattern = BackgroundType.DiagonalStripe;

            // Nuevo indicador de estilo
            StyleFlag styleFlag = new StyleFlag();

            // Establecer todos los estilos
            styleFlag.All = true;

            // Obtener primera columna
            Column column = worksheet.Cells.Columns[0];

            // Aplicar estilo a la primera columna
            column.ApplyStyle(style, styleFlag);

            // Configurando propiedades adicionales
            column.Width = 20.0; // Setting the column width
            column.IsHidden = false; // Setting the column visibility
            column.IsCollapsed = false; // Setting the column collapsed state

            // Guardando el archivo Excel
            workbook.Save("ColumnExample.xlsx");
            workbook.Save("ColumnExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


