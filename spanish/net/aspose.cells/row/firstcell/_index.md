---
title: "Row.FirstCell"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Row. Obtiene el primer objeto celda en la fila"
type: docs
url: /es/net/aspose.cells/row/firstcell/
---
## Row.FirstCell property

Obtiene el primer objeto celda en la fila.

```csharp
public Cell FirstCell { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyFirstCellDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos a las celdas en la primera fila
            worksheet.Cells["A1"].PutValue("First Cell");
            worksheet.Cells["B1"].PutValue("Second Cell");
            worksheet.Cells["C1"].PutValue("Third Cell");
            
            // Obtener la primera fila
            Row row = worksheet.Cells.Rows[0];
            
            // Demostrar la propiedad FirstCell
            Cell firstCell = row.FirstCell;
            Console.WriteLine("First cell in row: " + firstCell.Name + " with value: " + firstCell.StringValue);
            
            // Modificar la primera celda
            firstCell.PutValue("Modified First Cell");
            Console.WriteLine("Updated first cell value: " + firstCell.StringValue);
            
            // Guarda el libro de trabajo
            workbook.Save("RowFirstCellDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


