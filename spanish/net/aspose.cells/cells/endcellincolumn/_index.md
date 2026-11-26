---
title: "Cells.EndCellInColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Obtiene la última celda en esta columna"
type: docs
url: /es/net/aspose.cells/cells/endcellincolumn/
---
## EndCellInColumn(int) {#endcellincolumn}

Obtiene la última celda en esta columna.

```csharp
public Cell EndCellInColumn(int columnIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | Int32 | Índice de columna. |

### Valor de retorno

Objeto de celda.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodEndCellInColumnWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            worksheet.Cells["A4"].PutValue("Data3");
            worksheet.Cells["B1"].PutValue("Value1");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Obtén la última celda en la columna A (índice de columna 0)
            Cell lastCell = worksheet.Cells.EndCellInColumn(0);
            
            Console.WriteLine("Last cell in column A: Row " + lastCell.Row + ", Value: " + lastCell.StringValue);

            // Itera a través de todas las filas en la columna A
            for (int row = 0; row <= lastCell.Row; row++)
            {
                Cell cell = worksheet.Cells[row, 0];
                Console.WriteLine("Row " + row + ": " + cell.StringValue);
            }

            // Guarda el libro de trabajo
            workbook.Save("EndCellInColumnDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## EndCellInColumn(int, int, int, int) {#endcellincolumn_1}

Obtiene la última celda con el índice de columna máximo en este rango.

```csharp
public Cell EndCellInColumn(int startRow, int endRow, int startColumn, int endColumn)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | Int32 | Índice de fila inicial. |
| endRow | Int32 | Índice de fila final. |
| startColumn | Int32 | Índice de columna inicial. |
| endColumn | Int32 | Índice de columna final. |

### Valor de retorno

Objeto de celda.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodEndCellInColumnWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Pobla datos en la columna B (índice 1)
            worksheet.Cells[0, 1].PutValue("Data 1");
            worksheet.Cells[2, 1].PutValue("Data 2");
            worksheet.Cells[3, 1].PutValue("Data 3");

            try
            {
                // Llama a EndCellInColumn con los parámetros: startRow=0, endRow=5, startColumn=1, endColumn=1
                Cell result = worksheet.Cells.EndCellInColumn(0, 5, 1, 1);

                if (result != null)
                {
                    Console.WriteLine($"Last cell in column B between rows 0-5 is at row {result.Row}, column {result.Column}");
                    // Marca la celda encontrada
                    result.PutValue("Last Cell");
                    Style style = result.GetStyle();
                    style.Font.IsBold = true;
                    result.SetStyle(style);
                }
                else
                {
                    Console.WriteLine("No cells found in specified range");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing EndCellInColumn method: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("CellsMethodEndCellInColumnWithInt32Int32Int32Int32Demo.xlsx");
        }
    }
}
```

### Ver también

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


