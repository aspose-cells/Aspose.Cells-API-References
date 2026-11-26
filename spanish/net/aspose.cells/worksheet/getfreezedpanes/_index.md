---
title: "Worksheet.GetFreezedPanes"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de Worksheet. Obtiene los paneles congelados"
type: docs
url: /es/net/aspose.cells/worksheet/getfreezedpanes/
---
## Worksheet.GetFreezedPanes method

Obtiene los paneles congelados.

```csharp
public bool GetFreezedPanes(out int row, out int column, out int freezedRows, 
    out int freezedColumns)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32& | Índice de fila. |
| columna | Int32& | Índice de columna. |
| freezedRows | Int32& | Número de filas visibles en el panel superior, no más que el índice de fila. |
| freezedColumns | Int32& | Número de columnas visibles en el panel izquierdo, no más que el índice de columna. |

### Valor de retorno

Devuelve si la hoja de cálculo está congelada

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodGetFreezedPanesWithInt32ParametersDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Congelar paneles en la celda C5 (fila 4, columna 2) con 2 filas congeladas y 1 columna congelada
            worksheet.FreezePanes(4, 2, 2, 1);

            // Declarar variables para almacenar la información de los paneles congelados
            int row = 0;
            int column = 0;
            int freezedRows = 0;
            int freezedColumns = 0;

            try
            {
                // Llamar al método GetFreezedPanes con parámetros de salida
                bool hasFreeze = worksheet.GetFreezedPanes(out row, out column, out freezedRows, out freezedColumns);

                // Muestra los resultados
                Console.WriteLine("Worksheet has freeze panes: " + hasFreeze);
                if (hasFreeze)
                {
                    Console.WriteLine("Freeze position - Row: " + row + ", Column: " + column);
                    Console.WriteLine("Frozen rows: " + freezedRows + ", Frozen columns: " + freezedColumns);
                }

                // Guarda el libro de trabajo
                workbook.Save("WorksheetMethodGetFreezedPanesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFreezedPanes method: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


