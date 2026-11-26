---
title: "Cell.IsMerged"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cell. Comprueba si una celda forma parte de un rango combinado o no"
type: docs
url: /es/net/aspose.cells/cell/ismerged/
---
## Cell.IsMerged property

Comprueba si una celda forma parte de un rango combinado o no.

```csharp
public bool IsMerged { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsMergedDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Combinar celdas de A1 a B2
            worksheet.Cells.Merge(0, 0, 2, 2);

            // Comprobar si la celda A1 está combinada
            bool isMerged = worksheet.Cells["A1"].IsMerged;
            Console.WriteLine("Is cell A1 merged? " + isMerged);

            // Comprobar si la celda C1 está combinada (debería ser falso)
            isMerged = worksheet.Cells["C1"].IsMerged;
            Console.WriteLine("Is cell C1 merged? " + isMerged);

            // Guarda el libro de trabajo
            workbook.Save("MergedCellsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


