---
title: "Row.GetStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Row. Obtiene el estilo de esta fila"
type: docs
url: /es/net/aspose.cells/row/getstyle/
---
## Row.GetStyle method

Obtiene el estilo de esta fila.

```csharp
public Style GetStyle()
```

### Observaciones

Modificar directamente el objeto de estilo devuelto no tiene efecto en esta fila ni en ninguna celda de la misma. Debes llamar al método [`ApplyStyle`](../applystyle/) o [`SetStyle`](../setstyle/) para aplicar el cambio a esta fila. El estilo de la fila es el estilo que heredarán las celdas de esta fila (aquellas celdas que no tengan configuraciones de estilo personalizadas, como celdas existentes que no se les haya asignado un estilo explícitamente, o aquellas que no se hayan instanciado).

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowMethodGetStyleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establecer estilos para la demostración
            Style rowStyle = workbook.CreateStyle();
            rowStyle.Pattern = BackgroundType.Solid;
            rowStyle.ForegroundColor = System.Drawing.Color.Blue;
            cells.Rows[8].ApplyStyle(rowStyle, new StyleFlag { All = true });

            Style columnStyle = workbook.CreateStyle();
            columnStyle.Pattern = BackgroundType.Solid;
            columnStyle.ForegroundColor = System.Drawing.Color.Red;
            cells.Columns[5].ApplyStyle(columnStyle, new StyleFlag { All = true });

            // Demostrar el uso de GetStyle
            Style retrievedRowStyle = cells.Rows[8].GetStyle();
            Console.WriteLine("Row 8 Style - ForegroundColor: " + retrievedRowStyle.ForegroundColor);
            Console.WriteLine("Row 8 Style - Pattern: " + retrievedRowStyle.Pattern);

            Style retrievedColumnStyle = cells.Columns[5].GetStyle();
            Console.WriteLine("Column 5 Style - ForegroundColor: " + retrievedColumnStyle.ForegroundColor);
            Console.WriteLine("Column 5 Style - Pattern: " + retrievedColumnStyle.Pattern);
        }
    }
}
```

### Ver también

* class [Style](../../style/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


