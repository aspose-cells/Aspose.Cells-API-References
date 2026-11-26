---
title: "Cell.GetMergedRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cell. Devuelve un objeto Range que representa un rango combinado"
type: docs
url: /es/net/aspose.cells/cell/getmergedrange/
---
## Cell.GetMergedRange method

Devuelve un objeto [`Range`](../../range/) que representa un rango combinado.

```csharp
public Range GetMergedRange()
```

### Valor de retorno

[`Range`](../../range/) object. Null if this cell is not merged.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetMergedRangeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Combinar celdas
            cells.Merge(0, 0, 2, 2);

            // Obtener la primera celda
            Cell cell = cells[0, 0];

            // Obtener información del rango combinado
            Aspose.Cells.Range mergedRange = cell.GetMergedRange();
            
            // Mostrar los detalles del rango combinado
            Console.WriteLine("Merged Range Details:");
            Console.WriteLine($"First Row: {mergedRange.FirstRow}");
            Console.WriteLine($"First Column: {mergedRange.FirstColumn}");
            Console.WriteLine($"Row Count: {mergedRange.RowCount}");
            Console.WriteLine($"Column Count: {mergedRange.ColumnCount}");
        }
    }
}
```

### Ver también

* class [Range](../../range/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


