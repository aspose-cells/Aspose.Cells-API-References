---
title: "Cells.GetViewRowHeightInch"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Obtiene la altura de una fila especificada en unidades de pulgadas"
type: docs
url: /es/net/aspose.cells/cells/getviewrowheightinch/
---
## Cells.GetViewRowHeightInch method

Obtiene la altura de una fila especificada en unidades de pulgadas.

```csharp
public double GetViewRowHeightInch(int row)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | Índice de fila |

### Valor de retorno

Altura de la fila

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetViewRowHeightInchWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer altura de fila personalizada para la fila 2 en pulgadas
            worksheet.Cells.SetRowHeightInch(2, 1.5);

            try
            {
                // Llamar a GetViewRowHeightInch con el parámetro de índice de fila
                double rowHeight = worksheet.Cells.GetViewRowHeightInch(2);
                
                // Mostrar el resultado y verificar que la altura coincida con el valor establecido
                Console.WriteLine($"View row height of row 2: {rowHeight} inches");
                
                // Demostrar el efecto añadiendo contenido de muestra
                worksheet.Cells["A2"].PutValue($"Row Height: {rowHeight}\"");
                worksheet.Cells.SetColumnWidthInch(0, 15);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetViewRowHeightInch: {ex.Message}");
            }
            
            // Guardar el libro de trabajo modificado
            workbook.Save("CellsMethodGetViewRowHeightInchWithInt32Demo.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


