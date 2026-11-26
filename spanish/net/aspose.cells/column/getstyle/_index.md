---
title: "Column.GetStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Column. Obtiene el estilo de esta columna"
type: docs
url: /es/net/aspose.cells/column/getstyle/
---
## Column.GetStyle method

Obtiene el estilo de esta columna.

```csharp
public Style GetStyle()
```

### Observaciones

Modificar directamente el objeto de estilo devuelto no tiene efecto en esta columna ni en las celdas de esta columna. Debes llamar al método [`ApplyStyle`](../applystyle/) o [`SetStyle`](../setstyle/) para aplicar el cambio a esta columna. El estilo de la columna es el estilo que heredarán las celdas de esta columna (aquellas celdas que no tienen configuraciones de estilo personalizadas, como celdas existentes que no se les ha establecido un estilo explícitamente, o aquellas que no han sido instanciadas)

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnMethodGetStyleDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establecer estilo para la columna 5
            Style columnStyle = cells.Columns[5].GetStyle();
            columnStyle.Font.Name = "Arial";
            columnStyle.Font.Size = 14;
            columnStyle.Font.IsBold = true;
            cells.Columns[5].ApplyStyle(columnStyle, new StyleFlag { Font = true });

            // Establecer estilo para la fila 7
            Style rowStyle = cells.Rows[7].GetStyle();
            rowStyle.Font.Color = System.Drawing.Color.Red;
            rowStyle.Font.IsItalic = true;
            cells.Rows[7].ApplyStyle(rowStyle, new StyleFlag { Font = true });

            // Verificar el estilo de la columna
            Style retrievedColumnStyle = cells.Columns[5].GetStyle();
            Console.WriteLine("Column 5 Style:");
            Console.WriteLine($"Font: {retrievedColumnStyle.Font.Name}, Size: {retrievedColumnStyle.Font.Size}, Bold: {retrievedColumnStyle.Font.IsBold}");

            // Verificar el estilo de la fila
            Style retrievedRowStyle = cells.Rows[7].GetStyle();
            Console.WriteLine("\nRow 7 Style:");
            Console.WriteLine($"Color: {retrievedRowStyle.Font.Color}, Italic: {retrievedRowStyle.Font.IsItalic}");

            // Guarda el libro de trabajo
            workbook.Save("ColumnMethodGetStyleDemo_output.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../../style/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


