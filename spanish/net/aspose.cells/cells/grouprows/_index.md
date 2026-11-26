---
title: "Cells.GroupRows"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Agrupa filas"
type: docs
url: /es/net/aspose.cells/cells/grouprows/
---
## GroupRows(int, int, bool) {#grouprows_1}

Agrupa filas.

```csharp
public void GroupRows(int firstIndex, int lastIndex, bool isHidden)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstIndex | Int32 | El índice de la primera fila a agrupar. |
| lastIndex | Int32 | El índice de la última fila a agrupar. |
| isHidden | Booleano | Especifica si las filas agrupadas están ocultas. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGroupRowsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Poblar algunos datos
            for (int i = 0; i < 10; i++)
            {
                cells[i, 0].PutValue($"Group {i + 1}");
                for (int j = 1; j <= 5; j++)
                {
                    cells[i, j].PutValue($"Data {j}");
                }
            }

            // Agrupar filas 1 a 5 (índice basado en 0) y ocultarlas
            cells.GroupRows(1, 5, true);

            // Establecer fila de resumen debajo del grupo
            worksheet.Outline.SummaryRowBelow = false;

            // Guarda el libro de trabajo
            workbook.Save("GroupRowsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GroupRows(int, int) {#grouprows}

Agrupa filas.

```csharp
public void GroupRows(int firstIndex, int lastIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstIndex | Int32 | El índice de la primera fila a agrupar. |
| lastIndex | Int32 | El índice de la última fila a agrupar. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGroupRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Poblar algunos datos de muestra
            for (int i = 0; i < 10; i++)
            {
                cells[i, 0].PutValue("Row " + (i + 1));
            }

            // Agrupar filas 2 a 5 (índice basado en cero)
            cells.GroupRows(1, 4);

            // Guarda el libro de trabajo
            workbook.Save("GroupRowsExample.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


