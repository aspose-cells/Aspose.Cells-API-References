---
title: "Cells.UngroupRows"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Desagrupa filas"
type: docs
url: /es/net/aspose.cells/cells/ungrouprows/
---
## UngroupRows(int, int, bool) {#ungrouprows_1}

Desagrupa filas.

```csharp
public void UngroupRows(int firstIndex, int lastIndex, bool isAll)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstIndex | Int32 | El índice de la primera fila a desagrupar. |
| lastIndex | Int32 | El índice de la última fila a desagrupar. |
| isAll | Booleano | True, elimina toda la información agrupada. De lo contrario, elimina la información del grupo externo. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodUngroupRowsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear agrupaciones de filas anidadas para demostración
            worksheet.Cells.GroupRows(5, 7);  // First level grouping
            worksheet.Cells.GroupRows(5, 7);  // Second level grouping

            try
            {
                // Desagrupar todos los niveles de filas 5-7
                worksheet.Cells.UngroupRows(5, 7, true);

                Console.WriteLine("Rows 5-7 successfully ungrouped with all levels removed");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UngroupRows: {ex.Message}");
            }

            // Guardar el libro de trabajo modificado
            workbook.Save("UngroupRowsWithBooleanDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## UngroupRows(int, int) {#ungrouprows}

Desagrupa filas.

```csharp
public void UngroupRows(int firstIndex, int lastIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstIndex | Int32 | El índice de la primera fila a desagrupar. |
| lastIndex | Int32 | El índice de la última fila a desagrupar. |

### Observaciones

Solo elimina la información del grupo externo.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUngroupRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Poblar algunos datos
            for (int i = 0; i < 6; i++)
            {
                cells[i, 0].PutValue($"Row {i}");
            }

            // Agrupar filas 1 a 3 (índice basado en 0)
            cells.GroupRows(1, 3, true);

            Console.WriteLine("Rows grouped from index 1 to 3");

            // Desagrupar las mismas filas
            cells.UngroupRows(1, 3);

            Console.WriteLine("Rows ungrouped from index 1 to 3");

            // Guarda el libro de trabajo
            workbook.Save("UngroupRowsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


