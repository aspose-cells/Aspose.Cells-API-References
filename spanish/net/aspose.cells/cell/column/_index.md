---
title: "Cell.Column"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cell. Obtiene el número de columna basado en cero de la celda"
type: docs
url: /es/net/aspose.cells/cell/column/
---
## Cell.Column property

Obtiene el número de columna (basado en cero) de la celda.

```csharp
public int Column { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyColumnDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceda a las celdas y demuestre la propiedad Column
            Cell cell1 = worksheet.Cells["A1"];
            Cell cell2 = worksheet.Cells["B2"];
            Cell cell3 = worksheet.Cells["C3"];

            // Establecer valores y estilos
            cell1.PutValue("Cell A1");
            cell2.PutValue("Cell B2");
            cell3.PutValue("Cell C3");

            // Demostrar el uso de la propiedad Column
            Console.WriteLine("Cell A1 is in column: " + cell1.Column);
            Console.WriteLine("Cell B2 is in column: " + cell2.Column);
            Console.WriteLine("Cell C3 is in column: " + cell3.Column);

            // Modificar el ancho de columna usando la propiedad Column
            worksheet.Cells.Columns[cell1.Column].Width = 20;
            worksheet.Cells.Columns[cell2.Column].Width = 25;
            worksheet.Cells.Columns[cell3.Column].Width = 30;

            // Guarda el libro de trabajo
            workbook.Save("ColumnPropertyDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


