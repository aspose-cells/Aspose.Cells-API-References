---
title: "Cells.GetRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Obtiene el elemento Row en el índice de fila de celda especificado"
type: docs
url: /es/net/aspose.cells/cells/getrow/
---
## Cells.GetRow method

Obtiene el [`Row`](../../row/) elemento en el índice de fila de celda especificado.

```csharp
[Obsolete("Use Cells.CheckRow(int row) instead.")]
public Row GetRow(int row)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | Índice de fila |

### Valor de retorno

Si el objeto fila existe, devuelve el objeto Row; de lo contrario, devuelve null.

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice el método Cells.CheckRow(int row). Este método será eliminado 12 meses después desde febrero de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetRowWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea celdas en la fila 5 para asegurar que la fila exista
            worksheet.Cells["A5"].PutValue("Row 5 Data");
            worksheet.Cells["B5"].PutValue(12345);

            try
            {
                // Llama al método GetRow con el parámetro Int32
                Row resultRow = worksheet.Cells.GetRow(5);

                if (resultRow != null)
                {
                    // Demuestra la manipulación de filas
                    resultRow.Height = 20;
                    Console.WriteLine($"Retrieved row 5 successfully. Current height: {resultRow.Height} points");
                    
                    // Cuenta las celdas en la fila
                    int cellCount = 0;
                    foreach (Cell cell in resultRow)
                    {
                        cellCount++;
                    }
                    Console.WriteLine($"Row 5 contains {cellCount} cells");
                }
                else
                {
                    Console.WriteLine("Row 5 not found in worksheet");
                }
            }
            catch (ArgumentOutOfRangeException ex)
            {
                Console.WriteLine($"Invalid row index: {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRow: {ex.Message}");
            }

            // Guardar el libro de trabajo modificado
            workbook.Save("CellsMethodGetRowWithInt32Demo.xlsx");
        }
    }
}
```

### Ver también

* class [Row](../../row/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


