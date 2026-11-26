---
title: "Clase Row"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Row class. Representa una fila única en una hoja de cálculo"
type: docs
url: /es/net/aspose.cells/row/
---
## Row class

Representa una fila única en una hoja de cálculo.

```csharp
public class Row : IEnumerable
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [FirstCell](../../aspose.cells/row/firstcell/) { get; } | Obtiene el primer objeto celda en la fila. |
| [FirstDataCell](../../aspose.cells/row/firstdatacell/) { get; } | Obtiene la primera celda no vacía en la fila. |
| [GroupLevel](../../aspose.cells/row/grouplevel/) { get; set; } | Obtiene el nivel de grupo de la fila. |
| [HasCustomStyle](../../aspose.cells/row/hascustomstyle/) { get; } | Indica si esta fila tiene configuraciones de estilo personalizadas(diferentes de la predeterminada heredada del libro de trabajo). |
| [Height](../../aspose.cells/row/height/) { get; set; } | Obtiene y establece la altura de la fila en unidades de puntos. |
| [Index](../../aspose.cells/row/index/) { get; } | Obtiene el índice de esta fila. |
| [IsBlank](../../aspose.cells/row/isblank/) { get; } | Indica si la fila contiene datos. |
| [IsCollapsed](../../aspose.cells/row/iscollapsed/) { get; set; } | si la fila está colapsada |
| [IsHeightMatched](../../aspose.cells/row/isheightmatched/) { get; set; } | Indica si la altura de la fila coincide con la configuración de fuente predeterminada actual del libro. Verdadero en esta propiedad también indica que la altura de la fila es "automática" sin un valor de altura personalizado establecido por el usuario. |
| [IsHidden](../../aspose.cells/row/ishidden/) { get; set; } | Indica si la fila está oculta. |
| [Item](../../aspose.cells/row/item/) { get; } | Obtiene la celda. |
| [LastCell](../../aspose.cells/row/lastcell/) { get; } | Obtiene el último objeto de celda en la fila. |
| [LastDataCell](../../aspose.cells/row/lastdatacell/) { get; } | Obtiene la última celda no vacía en la fila. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [ApplyStyle](../../aspose.cells/row/applystyle/)(Style, StyleFlag) | Aplica formatos a toda la fila. |
| [CopySettings](../../aspose.cells/row/copysettings/)(Row, bool) | Copia la configuración de la fila, como estilo, altura, visibilidad, ...etc. |
| override [Equals](../../aspose.cells/row/equals/#equals_1)(object) | Comprueba si este objeto se refiere a la misma fila que otro. |
| [Equals](../../aspose.cells/row/equals/#equals)(Row) | Comprueba si este objeto se refiere a la misma fila que otro objeto de fila. |
| [GetCellByIndex](../../aspose.cells/row/getcellbyindex/)(int) | Obtiene la celda por un índice específico en la colección de celdas de esta fila. |
| [GetCellOrNull](../../aspose.cells/row/getcellornull/)(int) | Obtiene la celda o null en el índice específico. |
| [GetEnumerator](../../aspose.cells/row/getenumerator/#getenumerator)() | Obtiene el enumerador de celdas |
| [GetEnumerator](../../aspose.cells/row/getenumerator/#getenumerator_1)(bool, bool) | Obtiene un enumerador que recorre las celdas a través de esta fila. |
| [GetStyle](../../aspose.cells/row/getstyle/)() | Obtiene el estilo de esta fila. |
| [SetStyle](../../aspose.cells/row/setstyle/)(Style) | Establece el estilo de esta fila. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;
    using System.Collections;

    public class RowDemo
    {
        public static void RowExample()
        {
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();

            // Obteniendo la referencia de la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Cree un objeto de estilo
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

            // Obtener la primera fila
            Row row = worksheet.Cells.Rows[0];

            // Aplicar estilo a la primera fila
            row.ApplyStyle(style, styleFlag);

            // Estableciendo propiedades de la fila
            row.Height = 20.0;
            row.IsHidden = false;
            row.IsCollapsed = false;
            row.GroupLevel = 1;
            row.IsHeightMatched = true;

            // Accediendo a las celdas de la fila
            Cell firstCell = row.FirstCell;
            Cell firstDataCell = row.FirstDataCell;
            Cell lastCell = row.LastCell;
            Cell lastDataCell = row.LastDataCell;

            // Comprobando si la fila está vacía
            bool isBlank = row.IsBlank;

            // Comprobando si la fila tiene estilo personalizado
            bool hasCustomStyle = row.HasCustomStyle;

            // Obteniendo el índice de la fila
            int rowIndex = row.Index;

            // Obteniendo una celda por índice
            Cell cellByIndex = row.GetCellByIndex(0);

            // Obteniendo el estilo de la fila
            Style rowStyle = row.GetStyle();

            // Estableciendo el estilo de la fila
            row.SetStyle(rowStyle);

            // Copiando configuraciones de otra fila
            Row sourceRow = worksheet.Cells.Rows[1];
            row.CopySettings(sourceRow, true);

            // Enumerando las celdas de la fila
            IEnumerator cellEnumerator = row.GetEnumerator();
            while (cellEnumerator.MoveNext())
            {
                Cell cell = (Cell)cellEnumerator.Current;
                Console.WriteLine(cell.Name + ": " + cell.Value);
            }

            // Guardando el archivo Excel
            workbook.Save("RowExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


