---
title: "Cells.ShowGroupDetail"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Expande las filas/columnas agrupadas"
type: docs
url: /es/net/aspose.cells/cells/showgroupdetail/
---
## Cells.ShowGroupDetail method

Expande las filas/columnas agrupadas.

```csharp
public void ShowGroupDetail(bool isVertical, int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isVertical | Booleano | True, expande las filas agrupadas. |
| índice | Int32 | El índice de fila/columna |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodShowGroupDetailWithBooleanInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y acceder a la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rellenar datos de ejemplo en las filas 5-7 (índice basado en 0: 4-6)
            for (int row = 4; row <= 6; row++)
            {
                worksheet.Cells[row, 0].PutValue($"Row {row + 1}");
            }

            // Agrupar filas 4-6 (filas de Excel 5-7) y colapsarlas inicialmente
            worksheet.Cells.GroupRows(4, 6, true);

            try
            {
                // Expandir las filas agrupadas usando ShowGroupDetail (isVertical: false para filas, índice: 4)
                worksheet.Cells.ShowGroupDetail(false, 4);
                Console.WriteLine("ShowGroupDetail method executed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ShowGroupDetail: {ex.Message}");
            }

            // Guarda el libro de trabajo para demostrar el efecto
            workbook.Save("ShowGroupDetailWithBooleanInt32Demo.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


