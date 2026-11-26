---
title: "Cells.IsDeletingRangeEnabled"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Verifique si el rango puede ser eliminado"
type: docs
url: /es/net/aspose.cells/cells/isdeletingrangeenabled/
---
## Cells.IsDeletingRangeEnabled method

Comprueba si el rango puede ser eliminado.

```csharp
public bool IsDeletingRangeEnabled(int startRow, int startColumn, int totalRows, int totalColumns)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | Int32 | El índice de fila inicial del rango. |
| startColumn | Int32 | El índice de columna inicial del rango. |
| totalRows | Int32 | El número de filas en el rango. |
| totalColumns | Int32 | El número de columnas en el rango. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodIsDeletingRangeEnabledWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Rellene datos de ejemplo en las celdas A1:C5
            for (int row = 0; row < 5; row++)
            {
                for (int col = 0; col < 3; col++)
                {
                    cells[row, col].Value = $"Data{row}_{col}";
                }
            }

            try
            {
                // Verifique si la eliminación de 5 filas x 3 columnas a partir de A1 está habilitada
                bool canDelete = cells.IsDeletingRangeEnabled(0, 0, 5, 3);
                Console.WriteLine($"Can delete range: {canDelete}");

                if (canDelete)
                {
                    // Elimine el rango A1:C5 y desplace las celdas hacia arriba
                    cells.DeleteRange(0, 0, 4, 2, ShiftType.Up);
                    Console.WriteLine("Deleted range A1:C5 successfully");
                }

                workbook.Save("IsDeletingRangeEnabledOutput.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during range deletion: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


