---
title: "Cells.GetDependents"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Obtiene todas las celdas que hacen referencia a la celda específica"
type: docs
url: /es/net/aspose.cells/cells/getdependents/
---
## Cells.GetDependents method

Obtiene todas las celdas que hacen referencia a la celda específica.

```csharp
public Cell[] GetDependents(bool isAll, int row, int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isAll | Booleano | Indica si se deben comprobar otras hojas de cálculo |
| fila | Int32 | El índice de fila. |
| columna | Int32 | El índice de columna. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetDependentsWithBooleanInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Configura fórmulas y valores de muestra
            cells["A1"].PutValue(10);
            cells["B1"].Formula = "=A1*2";
            cells["C1"].Formula = "=A1+B1";
            cells["D1"].Formula = "=B1*3";
            cells["F4"].Formula = "=A1*5";

            // Calcular fórmulas
            workbook.CalculateFormula();

            // Obtener dependientes directos de la celda A1 (fila 0, columna 0)
            Cell[] directDependents = cells.GetDependents(false, 0, 0);
            Console.WriteLine("Direct dependents of A1:");
            foreach (Cell cell in directDependents)
            {
                Console.WriteLine(cell.Name);
            }

            // Obtener todos los dependientes (incluidos los indirectos) de la celda A1 (fila 0, columna 0)
            Cell[] allDependents = cells.GetDependents(true, 0, 0);
            Console.WriteLine("\nAll dependents of A1:");
            foreach (Cell cell in allDependents)
            {
                Console.WriteLine(cell.Name);
            }
        }
    }
}
```

### Ver también

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


