---
title: "Row.FirstDataCell"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Row. Obtiene la primera celda no vacía en la fila"
type: docs
url: /es/net/aspose.cells/row/firstdatacell/
---
## Row.FirstDataCell property

Obtiene la primera celda no vacía en la fila.

```csharp
public Cell FirstDataCell { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyFirstDataCellDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Colocar valores en diferentes celdas
            cells["A1"].PutValue("Header");
            cells["B2"].PutValue("FirstData");
            cells["C2"].PutValue("SecondData");
            
            // Obtener la primera celda de datos en la fila 1 (índice 0)
            Cell firstDataCellRow1 = cells.Rows[0].FirstDataCell;
            Console.WriteLine("First data cell in row 1: " + (firstDataCellRow1 != null ? firstDataCellRow1.Name : "null"));
            
            // Obtener la primera celda de datos en la fila 2 (índice 1)
            Cell firstDataCellRow2 = cells.Rows[1].FirstDataCell;
            Console.WriteLine("First data cell in row 2: " + firstDataCellRow2.Name);
        }
    }
}
```

### Ver también

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


