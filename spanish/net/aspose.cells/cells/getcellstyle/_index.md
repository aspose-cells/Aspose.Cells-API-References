---
title: "Cells.GetCellStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Obtener el estilo de la celda dada"
type: docs
url: /es/net/aspose.cells/cells/getcellstyle/
---
## Cells.GetCellStyle method

Obtiene el estilo de la celda dada.

```csharp
public Style GetCellStyle(int row, int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | índice de fila |
| columna | Int32 | columna |

### Valor de retorno

el estilo de la celda dada.

### Observaciones

El estilo devuelto es solo el que está establecido para la celda o heredado de la fila/columna de la celda, no incluye las propiedades aplicadas por otras configuraciones como los formatos condicionales.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellsMethodGetCellStyleWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder a la celda B5 (fila 4, columna 1) y establecer el estilo inicial
            Cell cell = worksheet.Cells["B5"];
            cell.PutValue("Styled Cell");
            
            // Crear y aplicar el estilo inicial de la celda
            Style initialStyle = workbook.CreateStyle();
            initialStyle.Font.IsBold = true;  // Changed from Bold to IsBold
            initialStyle.BackgroundColor = Color.LightYellow;
            cell.SetStyle(initialStyle);

            try
            {
                // Llamar a GetCellStyle con parámetros Int32 (fila 4, columna 1)
                Style cellStyle = worksheet.Cells.GetCellStyle(4, 1);

                // Mostrar las propiedades del estilo recuperado
                Console.WriteLine($"Retrieved style - Bold: {cellStyle.Font.IsBold}, Background: {cellStyle.BackgroundColor}");  // Changed from Bold to IsBold

                // Modificar el estilo recuperado
                cellStyle.Font.IsItalic = true;  // Changed from Italic to IsItalic
                cellStyle.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;

                // Aplicar el estilo modificado de nuevo a la celda
                cell.SetStyle(cellStyle);

                Console.WriteLine("GetCellStyle executed successfully. Modified border and font style.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellStyle: {ex.Message}");
            }

            // Guardar el libro de trabajo modificado
            workbook.Save("CellsGetCellStyleWithInt32Demo.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../../style/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


