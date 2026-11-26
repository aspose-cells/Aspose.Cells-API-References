---
title: "Cells.DeleteRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Elimina una fila"
type: docs
url: /es/net/aspose.cells/cells/deleterow/
---
## DeleteRow(int) {#deleterow}

Elimina una fila.

```csharp
public void DeleteRow(int rowIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | Int32 | Índice de la fila a eliminar. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteRowWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;

            // Establece una fórmula compartida en la fila 66
            cells[65, 0].SetSharedFormula("=SUM(B10:B66)", 1, 6);

            // Elimina la fila 9 (lo que desplazará las filas hacia arriba)
            cells.DeleteRow(9);

            // Verifica que la fórmula se ajustó después de la eliminación de la fila
            for (int i = 1; i < 7; i++)
            {
                char columnName = (char)('A' + i);
                Console.WriteLine($"Cell {columnName}66 formula after deletion: {cells[64, i].Formula}");
            }

            // Elimina las filas 60-61 (lo que desplazará las filas hacia arriba)
            cells.DeleteRows(59, 2);

            // Verifica que la fórmula se ajustó después de la eliminación de las filas
            for (int i = 1; i < 7; i++)
            {
                char columnName = (char)('A' + i);
                Console.WriteLine($"Cell {columnName}64 formula after deletion: {cells[62, i].Formula}");
            }
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteRow(int, bool) {#deleterow_1}

Elimina una fila.

```csharp
public void DeleteRow(int rowIndex, bool updateReference)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | Int32 | Índice de la fila a eliminar. |
| updateReference | Booleano | Indica si se actualizan referencias en otras hojas de cálculo. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteRowWithInt32BooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue("Item");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["A4"].PutValue("Cherry");

            Console.WriteLine("Original Data:");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(sheet.Cells[$"A{i}"].Value);
            }

            sheet.Cells.DeleteRow(2, true);

            Console.WriteLine("\nData After Deletion:");
            for (int i = 1; i <= 3; i++)
            {
                Console.WriteLine(sheet.Cells[$"A{i}"].Value);
            }

            workbook.Save("DeleteRowExample.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


