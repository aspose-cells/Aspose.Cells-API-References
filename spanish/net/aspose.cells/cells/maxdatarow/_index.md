---
title: "Cells.MaxDataRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cells. Índice máximo de fila de la celda que contiene datos"
type: docs
url: /es/net/aspose.cells/cells/maxdatarow/
---
## Cells.MaxDataRow property

Índice máximo de fila de la celda que contiene datos.

```csharp
public int MaxDataRow { get; }
```

### Observaciones

Devuelve -1 si no hay ninguna celda que contenga datos. Esta propiedad necesita iterar y comprobar celdas y filas de forma dinámica, por lo que es un proceso que consume tiempo y no debe invocarse repetidamente, como usarla directamente como condición en un bucle.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMaxDataRowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("Item1");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("Item2");
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["A4"].PutValue("Item3");
            sheet.Cells["B4"].PutValue(30);

            // Demostrar el uso de MaxDataRow
            int maxRow = sheet.Cells.MaxDataRow;
            Console.WriteLine("Max data row: " + maxRow);

            // Crear un área de celdas usando MaxDataRow
            int startRow = 0;
            int startColumn = 0;
            int endRow = sheet.Cells.MaxDataRow;
            int endColumn = sheet.Cells.MaxDataColumn;

            // Aplicar formato al rango de datos
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            
            // Aplicar estilo al rango
            sheet.Cells.CreateRange(startRow, startColumn, endRow + 1, endColumn + 1).ApplyStyle(style, new StyleFlag { FontBold = true });

            // Guarda el libro de trabajo
            workbook.Save("MaxDataRowDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


