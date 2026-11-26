---
title: "Cells.EndCellInRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Obtiene la última celda en esta fila"
type: docs
url: /es/net/aspose.cells/cells/endcellinrow/
---
## EndCellInRow(int) {#endcellinrow}

Obtiene la última celda en esta fila.

```csharp
public Cell EndCellInRow(int rowIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | Int32 | Índice de fila. |

### Valor de retorno

Objeto de celda.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodEndCellInRowWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Rellene datos en la fila 5 (índice basado en 0)
            worksheet.Cells[5, 2].PutValue("Data1");
            worksheet.Cells[5, 4].PutValue("Data2");
            worksheet.Cells[5, 6].PutValue("Data3");

            try
            {
                // Llame a EndCellInRow con el índice de fila 5
                Cell endCell = worksheet.Cells.EndCellInRow(5);
                
                if (endCell != null)
                {
                    Console.WriteLine($"Last cell in row 5: {endCell.Name}");
                    Console.WriteLine($"Cell value: {endCell.StringValue}");
                }
                else
                {
                    Console.WriteLine("No cells found in row 5");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing EndCellInRow: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("CellsMethodEndCellInRowWithInt32Demo.xlsx");
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

## EndCellInRow(int, int, int, int) {#endcellinrow_1}

Obtiene la última celda con el índice de fila máximo en este rango.

```csharp
public Cell EndCellInRow(int startRow, int endRow, int startColumn, int endColumn)
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
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodEndCellInRowWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Poblar algunos datos en la hoja de cálculo
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Cell_{i}_{j}");
                }
            }

            // Obtenga la celda final en la fila 3 entre las columnas 1 a 4
            Cell endCell = worksheet.Cells.EndCellInRow(3, 1, 3, 4);

            // Salida de los índices de fila y columna de la celda final
            Console.WriteLine($"End cell in row 3 between columns 1-4 is at: Row {endCell.Row}, Column {endCell.Column}");
        }
    }
}
```

### Ver también

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


