---
title: "Shape.GetLinkedCell"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Shape. Obtiene el rango vinculado al valor del control"
type: docs
url: /es/net/aspose.cells.drawing/shape/getlinkedcell/
---
## Shape.GetLinkedCell method

Obtiene el rango vinculado al valor del control.

```csharp
public string GetLinkedCell(bool isR1C1, bool isLocal)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isR1C1 | Booleano | Si la fórmula necesita formatearse como R1C1. |
| isLocal | Booleano | Si la fórmula necesita formatearse según la configuración regional. |

### Valor de retorno

El rango vinculado al valor del control.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetLinkedCellWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma y establecer su celda vinculada
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
            shape.LinkedCell = "A1";

            // Obtener la dirección de la celda vinculada con diferentes combinaciones de parámetros
            string link1 = shape.GetLinkedCell(false, false); // Returns absolute reference like "$A$1"
            string link2 = shape.GetLinkedCell(true, false);   // Returns relative reference like "A1"
            string link3 = shape.GetLinkedCell(false, true);   // Returns R1C1 style absolute reference

            Console.WriteLine("Linked cell (absolute A1): " + link1);
            Console.WriteLine("Linked cell (relative A1): " + link2);
            Console.WriteLine("Linked cell (R1C1 style): " + link3);
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


