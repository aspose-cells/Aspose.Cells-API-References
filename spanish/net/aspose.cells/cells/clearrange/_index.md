---
title: "Cells.ClearRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Elimina el contenido y el formato de un rango"
type: docs
url: /es/net/aspose.cells/cells/clearrange/
---
## ClearRange(CellArea) {#clearrange}

Borra el contenido y el formato de un rango.

```csharp
public void ClearRange(CellArea range)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rango | CellArea | Rango a eliminar. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodClearRangeWithCellAreaDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rellenar celdas con datos de ejemplo
            for (int row = 0; row <= 2; row++)
            {
                for (int col = 0; col <= 2; col++)
                {
                    worksheet.Cells[row, col].Value = $"Data_{row}_{col}";
                }
            }

            // Definir el CellArea a eliminar (filas 0-2, columnas 0-2)
            CellArea clearArea = new CellArea();
            clearArea.StartRow = 0;
            clearArea.EndRow = 2;
            clearArea.StartColumn = 0;
            clearArea.EndColumn = 2;

            try
            {
                // Eliminar el rango especificado
                worksheet.Cells.ClearRange(clearArea);
                Console.WriteLine("Cleared cells in range: Rows 0-2, Columns 0-2");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearRange method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("CellsMethodClearRangeWithCellAreaDemo.xlsx");
        }
    }
}
```

### Ver también

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ClearRange(int, int, int, int) {#clearrange_1}

Borra el contenido y el formato de un rango.

```csharp
public void ClearRange(int startRow, int startColumn, int endRow, int endColumn)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | Int32 | Índice de fila inicial. |
| startColumn | Int32 | Índice de columna inicial. |
| endRow | Int32 | Índice de fila final. |
| endColumn | Int32 | Índice de columna final. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodClearRangeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Poblar algunos datos de prueba
            cells[0, 0].PutValue(1);
            cells[0, 16383].PutValue(2);
            cells[1048575, 0].PutValue(3);
            cells[1048575, 16383].PutValue(4);

            // Eliminar todo el rango de la hoja de cálculo
            cells.ClearRange(0, 0, 1048575, 16383);

            // Guarda el libro de trabajo
            workbook.Save("ClearRangeDemo.xlsx");

            Console.WriteLine("ClearRange demo executed successfully.");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


