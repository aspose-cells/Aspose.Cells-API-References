---
title: "Row.LastDataCell"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Row. Obtiene la última celda no vacía en la fila"
type: docs
url: /es/net/aspose.cells/row/lastdatacell/
---
## Row.LastDataCell property

Obtiene la última celda no vacía en la fila.

```csharp
public Cell LastDataCell { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyLastDataCellDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Insertar datos en celdas
            cells["A1"].PutValue("First cell");
            cells["B1"].PutValue("Second cell");
            cells["C2"].PutValue("Not in first row");
            
            // Obtener la última celda de datos en la primera fila
            Cell lastDataCell = cells.Rows[0].LastDataCell;
            
            Console.WriteLine("Last data cell in first row: " + lastDataCell.Name);
            Console.WriteLine("Value in last data cell: " + lastDataCell.StringValue);
        }
    }
}
```

### Ver también

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


