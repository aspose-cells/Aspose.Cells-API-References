---
title: "Shape.GetInputRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Shape. Obtiene el rango utilizado para rellenar el control"
type: docs
url: /es/net/aspose.cells.drawing/shape/getinputrange/
---
## Shape.GetInputRange method

Obtiene el rango utilizado para rellenar el control.

```csharp
public string GetInputRange(bool isR1C1, bool isLocal)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isR1C1 | Booleano | Si la fórmula necesita formatearse como R1C1. |
| isLocal | Booleano | Si la fórmula necesita formatearse según la configuración regional. |

### Valor de retorno

El rango utilizado para rellenar el control.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetInputRangeWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("Input 1");
            worksheet.Cells["A2"].PutValue("Input 2");
            worksheet.Cells["A3"].PutValue("Input 3");

            // Agregar una forma de cuadro de lista
            ListBox listBox = (ListBox)worksheet.Shapes.AddListBox(0, 0, 100, 100, 0, 0);
            Shape shape = listBox;

            // Establecer el rango de entrada para el cuadro de lista
            shape.SetInputRange("$A$1:$A$3", false, false);

            // Obtener el rango de entrada
            string range = shape.GetInputRange(false, true);
            Console.WriteLine("Shape input range: " + range);
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


